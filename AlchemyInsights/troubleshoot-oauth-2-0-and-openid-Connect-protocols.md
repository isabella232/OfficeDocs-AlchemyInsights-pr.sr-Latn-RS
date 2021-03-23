---
title: Rešavanje problema sa aplikacijom OAuth 2,0 i OpenID povezivanja protokola
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037700"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Rešavanje problema sa aplikacijom OAuth 2,0 i OpenID povezivanja protokola

Da biste rešili OAuth 2,0 i OpenID probleme sa povezivanjem, obavite sledeće preporučene korake:

Pogledajte sledeće članke koji su povezani sa konfiguracijom i otklanjanju problema sa OAuth 2,0 i OpenID povezivanjem protokola:

- [Microsoft funkcija za identifikaciju identiteta i OAuth 2,0 protok koda](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – ovaj članak opisuje kako se programira **protok koda (pkće)** u aplikaciji pomoću bilo kog jezika.
- [Microsoft Platform identiteta i OAuth 2,0 akreditivi za klijenta](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – ovaj članak opisuje kako da se programira **protok akreditiva klijenta** u aplikaciji.
- [Microsoft Office Platform identiteta i OAuth 2,0 akreditivi za lozinku vlasnika resursa](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – ovaj članak opisuje kako se direktno programira **protok ropc** -a u aplikaciji.
    - Microsoft platforma za identifikaciju samo podržava ROPC za Azure AD zakupce i ne za lične naloge. To znači da morate da koristite krajnju tačku specifične za zakupca **( https://login.microsoftonline.com/{TenantId_or_Name})** ili krajnje tačke **organizacije** .
    - Lični nalozi koji su pozvani na Azure AD stanari ne mogu da koriste ROPC.
    - Nalozi koji nemaju lozinke ne mogu da se prijave kroz ROPC. Za ovaj scenario preporučujemo da koristite drugačiji protok za aplikaciju, umesto toga.
    - Ako je potrebno da korisnici koriste [multifaktor potvrdu identiteta (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) za prijavljivanje u aplikaciju, oni će biti blokirani.
    - ROPC nije podržan u [hibridnim slučajevima Federacije identiteta](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (na primer, AZURE AD i adfs koji se koriste za potvrdu autentičnosti lokalnog naloga). Ako su korisnici preusmjereni na lokalnog dobavljača identiteta, Azure AD nije u mogućnosti da testira korisničko ime i lozinku na tom dobavljaču identiteta. [Provera autentičnosti kroz proveru identiteta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) je podržana uz ropc.
    - Izuzetak sa scenariom hibridnog identiteta saveza će biti sledeće: smernice za otkrivanje preduzeća sa **Allowcloud Dpasha** -da biste **ostvarili na TRUE** OMOGUĆAVAĆE programu ropc da radi za ujedinjen korisnik kada se lokalna lozinka sinhronizuje sa oblakom. Više informacija potražite u članku [Omogućavanje direktnog ROPC identiteta povezanih korisnika za zastarele aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft Platform identiteta i OAuth 2,0 u interesu-](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) ovaj članak opisuje kako se direktno programira **protok u ime (OBO) toka** u aplikaciji.
- [Microsoft protokol za primenu identiteta i openid](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -ovaj članak prikazuje kako se sprovodi openid protokol povezivanja nezavisno od jezika i opisuje kako se šalju i primaju HTTP poruke bez korišćenja bilo koje Microsoft Open-izvorne biblioteke.

**Access simboli**

[Aplikacije Microsoft Access platforme za identifikaciju](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Saznajte kako API može da proveri valjanost i koristi zahteve unutar simbola za pristup. Sva dokumentacija u ovom članku, osim gde je navedeno, odnosi se samo na Tokene koji su izdati za APIs koje ste registrovali. Ne odnosi se na oznake koje su izdate za usluge koje posjeduje Microsoft-not, niti se ovi Tokeni mogu koristiti za validaciju načina na koji Microsoft platforma za identifikaciju izdaje tokena za API koji kreirate.

**Konfiguracija aplikacije**

[PREUSMERAVANJE Uri (URL adresa) ograničenja i ograničenja](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Saznajte kako da konfigurišete preusmeravanje Uri (URL adresa). Preusmeravanje URI ili URL adresa, jeste lokacija na kojoj server za autorizaciju šalje korisnika kada je aplikacija uspešno ovlašćena i dodeljena mu je kôd za autorizaciju ili Token za pristup. Server za ovlašćenje šalje kôd ili Token u preusmeravanje URI; Tako da je važno da registrujete tačnu lokaciju kao deo procesa registracije aplikacija.

**Obezbeđivanje aplikacije**

[Uputstvo: izrada i plan obezbeđivanje za scim krajnje tačke](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – ovaj članak opisuje kako se gradi krajim krajnje tačke i integriše se sa uslugom AAD obezbeđivanje.


