---
title: Potvrda identiteta
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
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019522"
---
# <a name="authentication-issues"></a>Potvrda identiteta

**Tražite informacije o AADSTS kodovima grešaka koji se vraćaju iz usluge sigurnosnih tokena Azure Active Directory (Azure AD) (STS)?** Pogledajte [Azure AD potvrdu identiteta i kodove grešaka](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) za pronalaženje AADSTS opisa grešaka, ispravki i nekih predloženih zaoštravanja.

Greške u autorizaciji mogu biti rezultat nekoliko različitih problema, od kojih većina generiše grešku 401 ili 403. Na primer, svi sledeći problemi mogu dovesti do grešaka u autorizaciji:

- Neispravno [tokovi prikupljanja tokena za pristup](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Loše konfigurisani[opsezi dozvola](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Da biste rešili uobičajene greške pri autorizaciji, isprobajte dolenavedene korake koji se najviše podudaraju sa greškom koju primate. Više koraka se može primeniti za grešku koju primate.

**Greška 401 neovlašćeno: Da li je vaš token važeći?**

Uverite se da vaša aplikacija predstavlja važeći token za pristup programu Microsoft Graph kao deo zahteva. Ova greška često znači da token za pristup možda nedostaje u zaglavlju zahteva za HTTP potvrdu identiteta ili da je token nevažeći ili je istekao. Preporučujemo vam da koristite Microsoft Authentication Library (MSAL) za prikupljanje pristupnih tokena. Pored toga, do ove greške može doći ako pokušate da koristite token za delegirani pristup dodeljen ličnom Microsoft nalogu za pristup API-ju koji podržava samo radne ili školske naloge (organizacione naloge).

**Greška 403 koja se odnosi na zabranu pristupa: Da li ste izabrali pravi skup dozvola?**

Uverite se da ste zatražili ispravan skup dozvola na osnovu API-ja Microsoft Graph koji vaša aplikacija poziva. Preporučene najmanje privilegovane dozvole su date u svim temama referentne metode Microsoft Graph API. Pored toga, te dozvole aplikaciji mora dodeliti korisnik ili administrator. Dodeljivanje dozvola obično se događa putem stranice saglasnosti ili upotrebe oštrice za registraciju aplikacije Azure Portal. U odeljku **Postavke** za aplikaciju kliknite na **Potrebne dozvole**, a zatim kliknite na **Odobri dozvole**. Za više informacija pogledajte članak:

- [Dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumevanje dozvola i saglasnosti za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Greška 403 koja se odnosi na zabranu pristupa: Da li je vaša aplikacija stekla token koji odgovara odabranim dozvolama?**

Uverite se da se vrste zahtevanih ili odobrenih dozvola podudaraju sa tipom tokena za pristup koji vaša aplikacija stiče. Možda zahtevate i dodeljujete dozvole za aplikacije, ali koristite delegirane interaktivne tokene toka koda umesto tokena protoka akreditiva klijenta ili tražite i dodeljujete delegirane dozvole, ali koristite tokene toka akreditiva klijenta umesto delegiranih tokena toka koda.

Za više informacija u vezi sa pribavljanjem tokena, pogledajte:

- [Pristupite u ime korisnika i delegiranih dozvola](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 – OAuth 2.0 tok koda autorizacije](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pristupite bez korisnika (usluga demona) i dozvola aplikacije](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 – OAuth 2.0 tok akreditiva klijenta](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Greška 403 koja se odnosi na zabranu pristupa: Resetovanje lozinke**

Trenutno ne postoji dozvola za aplikaciju za daemon dozvole usluge za uslugu koje omogućavaju uspostavljanje početnih vrednosti korisničkih lozinki. Ovi API-ji su podržani samo pomoću interaktivnih tokova delegiranog koda sa prijavljenim administratorom. Za više informacija pogledajte članak[ Microsoft Graph dozvole](https://docs.microsoft.com/graph/permissions-reference).

**Greška 403 koja se odnosi na zabranu pristupa: Da li korisnik ima pristup i da li ima licencu?**

Za tokove delegiranih kodova, Microsoft Graph procenjuje da li je zahtev dozvoljen na osnovu dozvola dodeljenih aplikaciji i dozvola koje ima prijavljeni korisnik. Generalno, ova greška ukazuje na to da korisnik nije dovoljno privilegovan da izvrši zahtev **ili** da nema licencu za podatke kojima se pristupa. Samo korisnici sa potrebnim dozvolama ili licencama mogu uspešno da podnesu zahtev.

**Greška 403 koja se odnosi na zabranu pristupa: Da li ste izabrali tačan API resursa?**

API usluge kao što je Microsoft Graph proveravaju da *aud* zahteva (publika) u primljenom tokenu za pristup odgovara vrednosti koju očekuje za sebe, a ako ne, pojavljuje se greška "Zabranjeno" 403. Uobičajena greška koja dovodi do ove greške je pokušaj korišćenja tokena stečenog za API-je Azure AD Graph, Outlook API ili SharePoint / OneDrive API za pozivanje Microsoft Graph-a (ili obrnuto). Uverite se da resurs (ili opseg) vaše aplikacije dobija token za podudaranje sa API-jem koji aplikacija poziva.

**400 Loš zahtev ili 403 zabranjeno: Da li je korisnik usaglašen sa smernicama za uslovni pristup organizacije (CA)?**

Na osnovu smernica uslovnog pristupa (CA) organizacije, korisnik koji pristupa resursima Microsoft Graph preko vaše aplikacije može biti osporavan zbog dodatnih informacija koje nisu prisutne u tokenu za pristup koji je vaša aplikacija prvobitno stekla. U ovom slučaju, vaša aplikacija prima **400 sa greškom *interaction_required*** tokom akvizicije pristupnog tokena ili **403 sa greškom *insufficient_claims*** prilikom pozivanja alatke Microsoft Graph. U oba slučaja odgovor na grešku sadrži dodatne informacije koje se mogu predstaviti ovlašćenoj krajnjoj tački da bi se korisnik pozvao na dodatne informacije (poput višefaktorske potvrde identiteta ili registracije uređaja).

Za više informacija u vezi sa uslovnim pristupom pogledajte članak:

- [Rešavanje izazova uslovnog pristupa pomoću MSAL-a](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Smernice za programere za uslovni pristup Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Kraj podrške za Azure Active Directory biblioteke potvrde identiteta (ADAL) i Azure AD Graph API (AAD Graph)***

- Od 30. juna 2020. više nećemo dodavati nove funkcije u Azure Active Directory Authentication Library (ADAL) i Azure AD Graph API (AAD Graph). Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.
- Od 30. juna 2022. prestaćemo sa podrškom za ADAL i AAD Graph i više nećemo pružati tehničku podršku ili bezbednosne ispravke.
    - Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da rade i nakon ovog vremena, ali neće dobiti nikakvu tehničku podršku ili bezbednosne ispravke.
    - Aplikacije koje koriste AAD Graph nakon ovog vremena možda više neće primati odgovore od krajnje tačke AAD Graph.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)koja ima najnovije funkcije i bezbednosne ispravke. Ova preporuka je u kontekstu Microsoft migracije svojih aplikacija na MSAL do krajnjeg roka za podršku. Cilj migracije Microsoft aplikacija na MSAL je da obezbedi da aplikacije imaju koristi od stalnih poboljšanja MSAL i zaštite.

- [Pročitajte najčešća pitanja za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Saznajte više o tome kako da migrirate aplikacije na osnovu platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ako vam je potrebna pomoć u razumevanju koja od vaših aplikacija koristi ADAL, preporučujemo vam da pregledate izvorni kod svih aplikacija i ako je primenljivo obratite se nezavisnim dobavljačima softvera (ISV) ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste AAD Graph, sledite naša uputstva za [migriranje aplikacija Azure AD Graph na Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Naša lista za migraciju pruža tačku za početak](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph. Preporučujemo vam da pregledate sav izvorni kod aplikacija i, ako je primenljivo, kontaktirate bilo koje ISV-ove ili dobavljače aplikacija. Microsoft podrška takođe može da vam pruži informacije o celokupnoj upotrebi AAD Graph kod vašeg zakupca.

 










