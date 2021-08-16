---
title: Problemi sa vezama i URL adresama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054812"
---
# <a name="issues-with-links-and-urls"></a>Problemi sa vezama i URL adresama

URI preusmeravanja/URL adrese odgovora (oba izraza su zamenljiva) predstavljaju URL adrese koje koristi Microsoft platforma za identitete da bi vratila tokene koje zahtevaju aplikacije. Više informacija o ovim URL adresama potražite u sledećim člancima:

- [Tokovi potvrde identiteta i scenariji aplikacija](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – Informacije o URI-ovima preusmeravanja na stranici **Registracija aplikacija** za svaki scenario.
- [Ograničenja URI-a preusmeravanja/URL adrese odgovora](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ne znam kako da registrujem odgovarajući URI preusmeravanja / URL adresu odgovora za svoju aplikaciju**

Kada se prijavite pomoću aplikacije koju projektujete, ako je u dijalogu za prijavljivanje prikazan tekst **AADSTS50011: URL adresa odgovora navedena u zahtevu ne podudara se sa URL adresama odgovora konfigurisanim za aplikaciju <your app ID>**, moraćete u registraciju aplikacije da dodate URI preusmeravanja koju je vaš kôd koristio u zahtevu za token za Microsoft platformu za identitete.

Da biste dodali URL adresu odgovora, idite na karticu **Potvrda identiteta** na stranici za **registraciju aplikacije** na Azure portalu i dodajte unos u odeljak **URI-ovi preusmeravanja**. Vrednost koju treba da unesete zavisi od tipa aplikacije koju projektujete, kao što je opisano u nastavku:

- Za aplikacije sa jednom stranicom i veb aplikacije, URL adresa odgovora je URL adresa u aplikaciji. Pogledajte članke [Registracija aplikacija sa jednom stranicom](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ili [Registracija veb aplikacije pomoću Azure portala](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Vrednost koju treba da odaberete za aplikacije za računare zavisi od:
    - platforme (MacOS se razlikuje od operativnog sistema Windows ili Linux)
    - načina na koji preuzimate token (interaktivno, pomoću toka koda uređaja, pomoću integrisane Windows potvrde identiteta [IWA] ili pomoću korisničkog imena/lozinke).
    Detalje potražite u odeljku [Aplikacije za računare – Registracija aplikacija – URI preusmeravanja](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Za aplikacije za mobilne uređaje, URI preusmeravanja zavisi od:
    - platforme (iOS/Android/UWP)
    - informacija koje se koriste za izgradnju aplikacije, kao što je ID kompleta u operativnom sistemu iOS, kao i ime paketa i hash potpisa u sistemu Android. Registracija aplikacija na Azure portalu će vam pomoći. Detalje potražite u odeljku [Konfiguracija platforme i URI-ovi preusmeravanja](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Veb API-ji i neki od tihih načina nabavke tokena (IWA i korisničko ime/lozinka) ne zahtevaju URI preusmeravanja.

**Projektovao/la sam svoju veb aplikaciji i prilikom testiranja primenjene aplikacije, dobijam poruku o nepodudaranju URL adresa odgovora**

Dodajte URI-ove preusmeravanja za sve lokacije na kojima primenjujete veb aplikaciju. Više informacija potražite u odeljku [Registrovanje veb aplikacije pomoću Azure portala](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Dodajte URI preusmeravanja za lokaciju odmah nakon primene aplikacije na toj lokaciji.

**Ne mogu da registrujem dovoljno URL adresa odgovora**

Vi ste ISV i imate jedan ili više URI-ova preusmeravanja za svakog od svojih klijenata. Želite da izvršite migraciju iz usluge ADAL/Azure AD v1.0 u MSAL/Microsoft platformu za identitete i dostigli ste [maksimalni broj URI-ova preusmeravanja](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Da biste rešili ovo, [dodajte URI-ove preusmeravanja u principale usluge](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) koji odgovaraju svakom od vaših klijenata.
