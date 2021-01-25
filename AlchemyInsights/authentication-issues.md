---
title: Problemi sa potvrdom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974793"
---
# <a name="authentication-issues"></a>Problemi sa potvrdom

**Tražite informacije o šifri greške AADSTS koje su vraćene iz usluge bezbednosnog koda Azure Active Directory (Azure AD)?** Pogledajte [Azure oglašavanje identiteta i lozinke kodova greške](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) da biste pronašli AADSTS opise grešaka, ispravke i neka predložena rešenja.

Greške pri autornosti mogu biti rezultat nekoliko raznih problema, od kojih većina stvara 401 ili 403 grešku. Na primer, sledeći problemi mogu sve da dovedu do grešaka autorizacije:

- Nepravilni [Tokovi nabavki za Access](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Slabo konfigurisani [Opsezi dozvola](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Manjak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Da biste rešili uobičajene greške pri autorizaciji, isprobajte korake navedene ispod koje se najviše podudara sa greškama koju primate. Više koraka može se primeniti na grešku koju primate.

- **401 neovlašćena greška: da li je simbol važeći?**

Uverite se da aplikacija predstavlja važeću Access Token u programu Microsoft Graph kao deo zahteva. Ova greška često znači da je u zaglavlju zahtjeva za pristup HTTP-u zahtev nestao i da je Token nevažeći ili da je istekao. Preporučujemo da koristite aplikaciju Microsoft biblioteke autentifikacije (MSAL) za preuzimanje oznaka Access. Pored toga, do ove greške može doći ako pokušate da koristite delegirani Access Token odobren ličnom Microsoft nalogu da biste pristupili API-ju koji podržava samo radne ili školske naloge (organizacioni nalozi).

**403 zabranjena greška: da li ste izabrali odgovarajući niz dozvola?**

Uverite se da ste zahtevali ispravan skupa dozvola na osnovu aplikacija Microsoft Graph API za vaše aplikacije. Preporučene najmanje privilegovane dozvole se pružaju u svim temama za Microsoft Graph API metode. Pored toga, na aplikaciju treba da odobri korisnik ili administrator. Odobravanje dozvola obično se dešava kroz stranicu sa dopuљtenja ili korišćenje oљtrice Azure aplikacije za Azure. Na oštrici **postavki** za aplikaciju izaberite stavku **obavezno dozvole**, a zatim izaberite stavku **Dodeli dozvole**. Za više informacija pogledajte članak:

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumevanje dozvola i pristanka Azure oglasa](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 zabranjena greška: da li je aplikacija priimala oznaku za podudaranje izabranih dozvola?**

Uverite se da su tipovi dozvola zahtevane ili dodeljene odgovaraju tipu oznake za Access koji aplikacija plaća. Možete da zahtevate i dodeljujete aplikacije, ali koristite dijazine akreditiva koda za klijentske uređaje, ali koristeći dijafrate akreditenih interaktivnog koda umesto jezičkog toka sadržaja klijenta.

Više informacija o pribavljanje tokena potražite u članku:

- [Nabavite pristup u ime korisnika i delegirane dozvole](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 protok koda autorizacije](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pristup pristupu bez korisnika (Daemon usluge) i dozvola za aplikacije](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0 – OAuth 2,0. akreditivi protoka klijenata](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 zabranjena greška: poništavanje lozinke**

Trenutno ne postoje dozvole za uslugu "demoni usluge za usluge" koje omogućava poništavanje korisničkih lozinki. Ovi API-ji su podržani samo pomoću interaktivne tokove delegiranog koda sa prijavljenim administratorom. Više informacija potražite u članku [dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 je zabranjen: da li korisnik ima pristup i da li su licencirani?**

Za delegirani tok koda, Microsoft Graph procenjuje da li je zahtev odobren na osnovu dozvola odobrenih aplikaciji i dozvolama koje ima prijavljeni korisnik. Ova greška obično ukazuje na to da korisnik nije dovoljno privilegovan da izvrši zahtev **ili** korisnik nije licenciran za pristup podacima. Zahtev može uspešno da sprovede samo korisnici sa potrebnim dozvolama ili licencama.

**403 je zabranjen: da li ste izabrali ispravan API resursa?**

Usluge API-ja kao što je Microsoft Graph uverite se da je *AUD* tvrdnja (publika) u primljenoj Access Token podudara se sa vrednošću koju ona očekuje za sebe i ako to ne uradi, javlja se greška u 403. Uobičajena greška koja dovodi do ove greške je korišćenje simbola koji se dobija za Azure AD Graph API, Outlook API-ju ili SharePoint/OneDrive API za poziv Microsoft Graph (ili obrnuto). Uverite se da je resurs (ili opseg) za aplikaciju pribavljanje simbola za podudaranje sa API koje aplikacija poziva.

**400 neispravan zahtev ili 403 je zabranjen: da li se korisnik slaže sa smernicama za uslovno pristup svoje organizacije?**

Na osnovu smernica za uslovni pristup (CA) organizacije, korisnik koji pristupa Microsoft Graph resursima pomoću aplikacije može da bude izazvan za dodatne informacije koje nisu prisutne u Token Access koji ste prvobitno nabavili. U ovom slučaju, aplikacija prima **400 sa *interaction_required*** greškama tokom kupovine Access oznake ili **403 pomoću *insufficient_claims*** greške prilikom poziva Microsoft Graph. U oba slučaja, odgovor na grešku sadrži dodatne informacije koje mogu biti predstavljene na pristupačnoj krajnjoj tački da bi se korisnik osporio za dodatne informacije (kao što je potvrda identiteta ili prijavljivanje uređaja).

Dodatne informacije o uslovnom pristupu potražite u članku:

- [Rukovanje uslovnim pristupom pomoću MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Vodič za projektovanje za uslovno aktivan pristup za Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Kraj podrške za Azure Active Directory potvrda identiteta biblioteke (ADALE) i AZURE AD Graph Graf (AAD Graph)_* _

- Počevši od 30 juna, 2020, više nećemo dodavati nijednu novu funkciju u biblioteku Azure aktivnog direktorijuma (ADALA) i API Azure AD Graph (AAD Graph). Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.
- Počevši od 30 juna, 2022, okončavamo podršku za ADALA i AAD Graf i više neće pružiti tehničku podršku ili bezbednosne ispravke.
    - Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće dobiti tehničku podršku ili bezbednosne ispravke.
    - Aplikacije koje koriste AAD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke AAD Graph.

/*Adala migracija**

Preporučujemo da ažurirate u [Microsoft biblioteci autentifikacije (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), koja ima najnovije funkcije i bezbednosne ispravke. Ova preporuka se nalazi u kontekstu Microsoft migriranja svojih aplikacija u MSAL po krajnjim rokovima. Cilj aplikacije "migracija Microsoft aplikacija u MSAL" jeste da biste se uverili da aplikacije imaju korist od tekuće bezbednosti i poboljšanja funkcija.

- [Pročitajte ADNO najčešća pitanja](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Saznajte kako da migrirate aplikacije na osnovu osnove po platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom nezavisnom dobavljaču proizvoda (ISVs) ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje ne podržavaju Microsoft u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste AAD Graph potražite uputstvo za [migraciju Azure AD Graph grafika u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Naša kontrolna lista za migraciju pruža taиku na početku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Vaš Azure registracioni portal pokazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija. Microsoft podrška vam pruža i informacije o korišćenju AAD Graph grafikona u vašem zakupcu.

 










