---
title: Problemi sa vezama i URL adresama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974752"
---
# <a name="issues-with-links-and-urls"></a>Problemi sa vezama i URL adresama

Preusmeravanje URI/odgovor URL adrese (oba izraza se mogu menjati) su URL adrese koje koristi Microsoft platforma za identifikaciju za povraćaj traženih željena aplikacija. Informacije o ovim URL adresama potražite u sledećim člancima:

- [Tokovi potvrde identiteta i scenariji aplikacije](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacije o preusmeravanju uris na stranici **registracija aplikacije** za svaki scenario.
- [Preusmeravanje URI/odgovori ograničenja URL adrese i ograničenja](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ne znam kako da registrujem pravo preusmeravanje JURIJ/odgovor URL za moju aplikaciju**

Kada se prijavite pomoću aplikacije koju razvijate, ako dijalog za prijavljivanje prikazuje **AADSTS50011: URL adresa odgovora navedena u zahtevu se ne podudara sa URL adresama koje su podešene za aplikaciju <your app ID>**, moraćete da dodate registraciju aplikacije, preusmeravanje i da kôd koji koristite u zahtevu za oznaku Microsoft identiteta.

Da biste dodali URL za odgovor, idite na karticu **potvrda identiteta** na stranici **registracija aplikacije** na Azure portalu i dodajte stavku u odeljak **preusmeravanja uris** . Preusmeri Urove su otkucane (Veb ili mobilna/radna površina). Vrednost koju treba da unesete zavisi od tipa aplikacije koju gradite, kao što je opisano ispod:

- Za aplikacije sa jednom stranicom i Veb aplikacijama, URL adresa je URL adresa u aplikaciji. Pogledajte [registraciju aplikacije sa jednom stranicom](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ili [Registrujte aplikaciju Veb aplikacije pomoću Azure portala](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Za aplikacije za stone računare vrednost koju treba da odaberete zavisi od:
    - platforma (MacOS se razlikuje od Windowsa ili Linux)
    - način na koji ste nabavili simbol (interaktivno, uz protok koda uređaja, sa integrisanom Windows autentifikacijom [IWA] ili sa korisničkim imenom/lozinkom).
    Detalje potražite u članku [aplikacije za računare – registracija aplikacije – preusmeravanje URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Za mobilne aplikacije, URI preusmeravanje zavisi od:
    - platforma (iOS/Android/UWP)
    - informacije koje se koriste za izradu aplikacije, kao što je ID za spakuju u iOS, kao i hash ime paketa i hash na usluzi android, Registracija na Azure će vam pomoći. Detalje potražite u članku [Konfigurisanje platforme i preusmeravanje ure](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Veb API i neke od tihog načina za sticanje tokena (IWA i username/password) ne zahtevaju preusmeravanje URI.

**Rasporedio sam Veb aplikaciju i kada sam testirao aplikaciju "raspoređeno", dobijam poruku "pogrešno podudaranje sa URL adresom"**

Dodajte preusmeravanje za sve lokacije na kojima koristite Veb aplikaciju. Više informacija potražite u članku [Registrovanje aplikacije Veb aplikacije pomoću Azure portala](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Dodajte preusmeravanje URI za lokaciju neposredno posle primene aplikacije na toj lokaciji.

**Ne mogu da registrujem dovoljno URL adrese odgovora**

Vi ste ISV i imate jedan ili više Urova za preusmeravanje za svaku vašu muљteriju. Želite da migrirate iz ADAL/Azure AD v 1.0 u MSAL/Microsoft Platform identiteta i pritisnite [Maksimalan broj preusmeravanja ure](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Da biste rešili ovo, [Dodajte preusmeravanje URIs za servisne direktore](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) koji odgovaraju svakom od vaših klijenata.
