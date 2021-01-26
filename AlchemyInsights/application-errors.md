---
title: Greške aplikacije
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984660"
---
# <a name="application-errors"></a>Greške aplikacije

Tražite informacije o **šifri greške Aadsts** koje su vraćene iz usluge bezbednosnog koda Azure Active Directory (AZURE AD)? Pročitajte [Azure oglase identiteta i lozinke kodova grešaka](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) da biste pronašli AADSTS opise grešaka, ispravke i neka predložena rešenja.

Greške pri autornosti mogu biti rezultat nekoliko raznih problema, od kojih većina stvara 401 ili 403 grešku. Na primer, sledeće mogu sve da dovedu do grešaka autorizacije:

- Nepravilni [Tokovi nabavki za Access](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Slabo konfigurisani [Opsezi dozvola](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Manjak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Da biste rešili uobičajene greške pri autorizaciji, isprobajte korake navedene ispod koji se najviše podudara sa greškama koju primate. Može se primeniti više od jednog.

**401 neovlašćena greška: da li je simbol važeći?**

Uverite se da aplikacija predstavlja važeću Access Token u programu Microsoft Graph kao deo zahteva. Ova greška često znači da je u zaglavlju zahtjeva za pristup HTTP-u zahtev nestao i da je Token nevažeći ili da je istekao. Preporučujemo da koristite aplikaciju [Microsoft biblioteke autentifikacije (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) za preuzimanje oznaka Access. Pored toga, do ove greške može doći ako pokušate da koristite delegirani Access Token odobren ličnom Microsoft nalogu da biste pristupili API-ju koji podržava samo radne ili školske naloge (organizacioni nalozi).

**403 zabranjena greška: da li ste izabrali odgovarajući niz dozvola?**

Potvrdite da ste zahtevali ispravan skupa dozvola na osnovu Microsoft Graph API vaših aplikacija. Preporučene najmanje privilegovane dozvole se pružaju u svim temama za Microsoft Graph API metode. Pored toga, na aplikaciju treba da odobri korisnik ili administrator. Dodeljivanje dozvola se obično odvija kroz stavku pristanak ili dodeljivanja dozvola pomoću oљtrice Azure registracije portala. Na oštrici **postavki** za aplikaciju izaberite stavku **obavezno dozvole**, a zatim izaberite stavku **Dodeli dozvole**.

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumevanje dozvola i pristanka Azure oglasa](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 zabranjena greška: da li je aplikacija priimala oznaku za podudaranje izabranih dozvola?**

Uverite se da su zahtevani tipovi dozvola ili dodeljene koji odgovaraju tipu oznake za pristup koje aplikacija plaća. Možete da zahtevate i dodeljujete dozvole za aplikacije, ali koristite iskre delegiranih interaktivnih tokova koda umesto jezičkog toka akreditiva klijenta, ili zahtevanje i dodeljivanje delegiranih dozvola, ali pomoću tokena protoka koda klijenta.

- [Nabavite pristup u ime korisnika i delegirane dozvole](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 protok koda autorizacije](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pristup pristupu bez korisnika (Daemon usluge) i dozvola za aplikacije](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0 – OAuth 2,0. akreditivi protoka klijenata](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 zabranjena greška: poništavanje lozinke**

Trenutno ne postoje dozvole za uslugu "demoni usluge za usluge" koje omogućava poništavanje korisničkih lozinki. Ovi API-ji su podržani samo pomoću interaktivne tokove delegiranog koda sa prijavljenim administratorom.

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 je zabranjen: da li korisnik ima pristup i da li su licencirani?**

Za delegirani tok koda, Microsoft Graph procenjuje da li je zahtev dozvoljen na osnovu dozvola dodeljenim aplikaciji i dozvolama koje ima prijavljeni korisnik. Ova greška obično ukazuje na to da korisnik nije dovoljno privilegovan da izvrši zahtev ili korisnik nije licenciran za pristup podacima. Zahtev može uspešno da sprovede samo korisnici sa potrebnim dozvolama ili licencama.

**403 je zabranjen: da li ste izabrali ispravan API resursa?**

API usluge kao što je Microsoft Graph proveravaju da li će AUD tvrdnja (publika) u primljenoj Access oznaku se podudara sa vrednošću koju ona očekuje sama za sebe, a ako ne, ona će biti u 403 zabrani. Uobičajena greška koja dovodi do ove greške je korišćenje simbola koji se dobija za Azure AD Graph API, Outlook API-ju ili SharePoint/OneDrive API za poziv Microsoft Graph (ili obrnuto). Uverite se da je resurs (ili opseg) za aplikaciju pribavljanje simbola za podudaranje sa API koje aplikacija poziva.

**400 neispravan zahtev ili 403 je zabranjen: da li se korisnik slaže sa smernicama za uslovno pristup svoje organizacije?**

Na osnovu ke smernice organizacije, korisnik koji pristupa Microsoft Graph resursima pomoću aplikacije može biti izazvan za dodatne informacije koje nisu prisutne u Token Access oznake koju je aplikacija prvobitno stekla. U ovom slučaju, aplikacija prima 400 sa *interaction_required* greškama tokom kupovine Access oznake ili 403 pomoću *insufficient_claims* greške prilikom poziva Microsoft Graph. U oba slučaja, odgovor na grešku sadrži dodatne informacije koje mogu biti predstavljene na krajnjoj tački ovlašćenja da bi se izazvao korisnik za dodatne informacije (kao što je potvrda identiteta ili prijavljivanje uređaja).

- [Rukovanje uslovnim pristupom pomoću MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Vodič za projektovanje za uslovno aktivan pristup za Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
