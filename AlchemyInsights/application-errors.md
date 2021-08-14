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
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931463"
---
# <a name="application-errors"></a>Greške aplikacije

Tražite informacije o **AADSTS** kodovima grešaka koji se vraćaju iz bezbednosne usluge tokena Azure Active Directory (Azure AD) (STS)? Pročitajte [Azure AD Authentication](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) i kôd greške autorizacije da biste pronašli AADSTS opise grešaka, ispravke i neka predložena zaoštravanja.

Greške u autorizaciji mogu biti rezultat nekoliko različitih problema, od kojih većina generiše grešku 401 ili 403. Na primer, sve sledeće može dovesti do grešaka u autorizovanju:

- Neispravno [tokovi prikupljanja tokena za pristup](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Loše konfigurisani[opsezi dozvola](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Da biste otklonili uobičajene greške u autorizovanju, isprobajte dole navedene korake koji najviše odgovaraju grešci koju primate. Može se primeniti više njih.

**Greška 401 neovlašćeno: Da li je vaš token važeći?**

Uverite se da aplikacija predstavlja važeći token za pristup korporaciji Microsoft Graph u sklopu zahteva. Ova greška često znači da token za pristup možda nedostaje u zaglavlju zahteva za HTTP potvrdu identiteta ili da je token nevažeći ili je istekao. Preporučujemo da koristite [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) za pristup tokenu za pristup. Pored toga, do ove greške može doći ako pokušate da koristite token za delegiran pristup dodeljen ličnom Microsoft nalogu za pristup API-u koji podržava samo radne ili školske naloge (naloge organizacije).

**Greška 403 koja se odnosi na zabranu pristupa: Da li ste izabrali pravi skup dozvola?**

Proverite da li ste zatražili odgovarajući skup dozvola na osnovu Microsoft Graph APIS-ja poziva vaše aplikacije. Preporučene dozvole sa najmanje privilegije pružene su u svim Temama Graph Microsoft Graph API metoda reference. Pored toga, te dozvole aplikaciji mora dodeliti korisnik ili administrator. Dodeljvanje dozvola obično se odvija putem stranice pristanka ili dodeljivanjem dozvola pomoću blejda za registraciju aplikacije Azure Portal. U odeljku **Postavke** za aplikaciju kliknite na **Potrebne dozvole**, a zatim kliknite na **Odobri dozvole**.

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumevanje dozvola i saglasnosti za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Greška 403 koja se odnosi na zabranu pristupa: Da li je vaša aplikacija stekla token koji odgovara odabranim dozvolama?**

Proverite da li se tip traženih ili dodeljenih dozvola podudara sa tipom tokena za pristup koji preuzima aplikacija. Možda zahtevate i dodelavate dozvole za aplikaciju, ali koristite delegirane tokene tokova koda umesto tokena toka akreditiva klijenta ili zahtevate i dodeljujte delegirane dozvole, ali koristite tokene akreditiva klijenta umesto delegiranih tokova toka koda.

- [Pristupite u ime korisnika i delegiranih dozvola](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 – OAuth 2.0 tok koda autorizacije](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pristupite bez korisnika (usluga demona) i dozvola aplikacije](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 – OAuth 2.0 tok akreditiva klijenta](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Greška 403 koja se odnosi na zabranu pristupa: Resetovanje lozinke**

Trenutno ne postoji dozvola za aplikaciju za daemon dozvole usluge za uslugu koje omogućavaju uspostavljanje početnih vrednosti korisničkih lozinki. Ovi API-ji su podržani samo pomoću interaktivnih tokova delegiranog koda sa prijavljenim administratorom.

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**Greška 403 koja se odnosi na zabranu pristupa: Da li korisnik ima pristup i da li ima licencu?**

Za delegirane tokove koda Microsoft Graph procenjuje da li je zahtev dozvoljen na osnovu dozvola dodeljenih aplikaciji i dozvola koje ima prijavljeni korisnik. Generalno, ova greška ukazuje na to da korisnik nije dovoljno privilegovan da izvrši zahtev ili da nema licencu za podatke kojima se pristupa. Samo korisnici sa potrebnim dozvolama ili licencama mogu uspešno da podnesu zahtev.

**Greška 403 koja se odnosi na zabranu pristupa: Da li ste izabrali tačan API resursa?**

API usluge kao što su Microsoft Graph proveravaju da li aud zahtev (publika) u tokenu primljenog pristupa odgovara vrednosti koju očekuje za sebe, a ako ne, to daje grešku "Zabranjeno" 403. Uobičajena greška koja dovodi do ove greške je pokušaj korišćenja tokena stečenog za API-je Azure AD Graph, Outlook API ili SharePoint / OneDrive API za pozivanje Microsoft Graph-a (ili obrnuto). Uverite se da resurs (ili opseg) vaše aplikacije dobija token za podudaranje sa API-jem koji aplikacija poziva.

**400 Loš zahtev ili 403 zabranjeno: Da li je korisnik usaglašen sa smernicama za uslovni pristup organizacije (CA)?**

Na osnovu SMERNICA ORGANIZACIJE, korisnik koji pristupa Microsoft Graph resursima putem aplikacije može biti izazovan za dodatne informacije koje nisu prisutne u tokenu pristupa koji je aplikacija prvobitno preuzeta. U ovom slučaju, vaša aplikacija prima 400 sa greškom *interaction_required* tokom akvizicije pristupnog tokena ili 403 sa greškom *insufficient_claims* prilikom pozivanja alatke Microsoft Graph. U oba slučaja odgovor na grešku sadrži dodatne informacije koje se mogu predstaviti krajnjim tačkama autorizovanja da bi se korisnik osporio zbog dodatnih informacija (kao što je višestruka potvrda identiteta ili unošenje uređaja).

- [Rukovanje izazovima uslovnog pristupa pomoću MSAL-a ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Smernice za programere za uslovni pristup Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
