---
title: Problemi sa vezom SSO
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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935158"
---
# <a name="sso-connection-issues"></a>Problemi sa vezom SSO

1. Izvršite [brzi Start: Konfigurišite svojstva vodiča za aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) da biste konfigurisali aplikaciju.
2. U zavisnosti od aplikacije i [Opcije za jedinstveno prijavljivanje](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) koje ste odabrali, idite ispod odgovarajućih uputstava:
    - Da biste konfigurisali **lokalnu aplikaciju** za **jedinstveno prijavljivanje u saml-u**, pogledajte [Sal jednokratni prijavljivanje za lokalne aplikacije pomoću proxy servera](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Da biste konfigurisali **aplikaciju oblaka** za **jedinstveno prijavljivanje na lozinku**, pogledajte članak  [Konfigurisanje jedinstvenog prijavljivanja lozinki](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Da biste konfigurisali **lokalnu aplikaciju** za **jedinstveno prijavljivanje kroz proxy server**, pogledajte članak podešavanje [lozinki za jedinstveno prijavljivanje pomoću proxy servera](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Problemi sa proxy** serverom za rešavanje problema: preporučujemo vam da počnete sa pregledanjem toka problema, otklanjanju problema sa proxy serverom za [otklanjanje grešaka](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), da biste utvrdili da li su konektori proxy servera ispravno konfigurisani. Ako i dalje imate problema prilikom povezivanja sa aplikacijom, slede tok rešavanja problema u [problemima sa proxy aplikacijom za Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Imate [probleme sa KORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomoću pregledača za otklanjanje grešaka:
    - Pokrenite pregledač i potražite Veb aplikaciju.
    - Pritisnite kombinaciju tastera **F12** da biste doveli konzolu za otklanjanje grešaka.
    - Pokušajte da reprodukujete transakciju i Pregledajte poruku konzole. Kršenje KORS daje grešku konzole o poreklu.
    - Neke CORS probleme ne možete da razrešite, na primer kada aplikacija preusmerava na login.microsoft.com za potvrdu identiteta, a ističe Access Token. KOROVI poziv je zatim propao. Rešenje za ovaj scenario je da produžite životni vek Token Access, da biste ga sprečili da ističe tokom sesije korisnika. Više informacija o tome kako da to uradite potražite u članku broj ћivota koji je [moguće konfigurisati u Microsoft platformi identiteta](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Rešavanje problema sa jednostrukim prijavljivanjem iz SAML-** a: preporučujemo da proverite [probleme sa prijavljivanjem u samla zasnovane na jedinstvenom prijavljivanju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)za pronalaženje rešenja za probleme na koje možete da naiđete.
5. **Rešavanje problema sa jedinstvenim prijavljivanjem zasnovanim na lozinci**: preporučujemo da proverite [Rešavanje problema sa jedinstvenim prijavljivanjem zasnovanim na lozinci u usluzi Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), da biste pronašli rešenja za pitanja na koja ćete se najverovatnije susretati.
6. Za probleme sa vezom prilikom korišćenja VPN-a pogledajte članak [Korišćenje jedinstvenog prijavljivanja (SSO) preko VPN-a i Wi-Fi veza](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
