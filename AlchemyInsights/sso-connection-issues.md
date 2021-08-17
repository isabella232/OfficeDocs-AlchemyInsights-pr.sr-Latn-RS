---
title: Problemi sa SSO vezom
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084360"
---
# <a name="sso-connection-issues"></a>Problemi sa SSO vezom

1. Pratite [brzi start: Konfigurišite svojstva za vodič za aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) da biste konfigurisali aplikaciju.
2. U zavisnosti od aplikacije i opcije [jedinstvenog prijavljivanje koju ste odabrali,](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) pratite odgovarajuća uputstva ispod:
    - Da biste  konfigurisali pojedinačno prijavljivanje zasnovanu na [SAML-u,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)pogledajte temu Jedinstveno prijavljivanje ZA **SAML** za aplikacije sa proxy serverom aplikacije.
    - Da biste **konfigurisali aplikaciju u** **oblaku za** jedinstveno prijavljivanje zasnovano na lozinki, pogledajte konfigurisanje jedinstvenog prijavljivanje [lozinkom.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Da biste **konfigurisali** jednu aplikaciju za jedinstveno prijavljivanje preko proxy servera **aplikacije,** pogledajte trezor lozinke za jedinstveno prijavljivanje sa proxy [serverom aplikacije.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. Rešavanje problema sa **proxy** serverom aplikacije: preporučujemo da počnete sa pregledanjem toka rešavanja problema, otklanjanja grešaka sa [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)konektorom aplikacije , da biste utvrdili da li su konektori proxy servera aplikacije ispravno konfigurisani. Ako i dalje imate problema pri povezivanju sa aplikacijom, pratite tok rešavanja problema u aplikaciji Otklanjanje grešaka u aplikaciji [Proxy aplikacije za otklanjanje grešaka.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) CorS probleme možete [da identifikujete pomoću alatki](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) za otklanjanje grešaka u pregledaču:
    - Pokrenite pregledač i potražite veb aplikaciju.
    - Pritisnite **taster F12 da** biste pojavili konzolu za otklanjanje grešaka.
    - Pokušajte da ponovo predstavite transakciju i pregledajte poruku konzole. Kršenje pravila CORS-a proizvodi grešku konzole u vezi sa poreklom.
    - Neke probleme sa aplikacijom CORS nije moći da rešite, na primer kada aplikacija preusmerava aplikaciju login.microsoft.com da potvrdi identitet, a token za pristup ističe. CORS poziv zatim ne uspeva. Zaokupno za ovaj scenario jeste da produžite trajanje tokena za pristup kako biste sprečili da on bude duži tokom sesije korisnika. Dodatne informacije o tome kako to da uradite potražite u temi Konfigurisanje trajanja [tokena](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)koji je Microsoft platforma za identitete.
4. Rešavanje problema sa jedinstvenim prijavljivanjem zasnovanim na **SAML-u:** preporučujemo da proverite probleme sa prijavljivanjem u aplikacije konfigurisane za jedinstveno prijavljivanje zasnovane na [SAML-u](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)kako biste pronašli rešenja za probleme na koje ćete najverovatnije naići.
5. Rešavanje problema sa jedinstvenim prijavljivanjem zasnovanim na lozinki: preporučujemo da proverite Rešavanje problema sa jedinstvenim prijavljivanjem zasnovanim na lozinki u [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), da biste pronašli rešenja za probleme na koje ćete najverovatnije naići.
6. Za probleme sa vezom prilikom korišćenja VPN-a pogledajte kako da koristite jedinstveno prijavljivanje [(SSO) preko VPN-a Wi-Fi veza.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
