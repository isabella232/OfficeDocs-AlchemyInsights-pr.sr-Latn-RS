---
title: Problemi sa integrisanjem nesomećenog SSO-a sa mojim ugrađenim aplikacijama
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028306"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemi sa integrisanjem nesomećenog SSO-a sa mojim ugrađenim aplikacijama

Da biste rešili probleme sa integrisanjem nesomećenog SSO-a sa primenjenim aplikacijama, uradite sledeće:

**Preporučeni koraci**

1. Da biste **konfigurisali** jednu aplikaciju za jedinstveno prijavljivanje preko proxy servera **aplikacije,** pogledajte trezor lozinke za jedinstveno prijavljivanje sa proxy [serverom aplikacije.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. Rešavanje problema sa **proxy** serverom aplikacije: preporučujemo da počnete sa redigovanju toka rešavanja [problema,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problemi sa proxy konektorom aplikacije za otklanjanje grešaka da biste utvrdili da li su konektori proxy aplikacije ispravno konfigurisani. Ako i dalje imate problema pri povezivanju sa aplikacijom, pratite korake za rešavanje problema u odeljku Otklanjanje problema sa proxy aplikacijom aplikacije za [otklanjanje grešaka.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) CorS probleme možete [da identifikujete pomoću](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) sledećih alatki za otklanjanje grešaka u pregledaču:
    1. Pokrenite pregledač i potražite veb aplikaciju.
    1. Pritisnite **taster F12 da** biste pojavili konzolu za otklanjanje grešaka.
    1. Pokušajte da ponovo predstavite transakciju i pregledajte poruku konzole. Kršenje pravila CORS-a proizvodi grešku konzole u vezi sa poreklom.
    1. Neke probleme sa aplikacijom CORS nije moći da rešite, na primer kada aplikacija preusmerava na potvrdu identiteta login.microsoftonline.com, a token za pristup ističe. CORS poziv zatim ne uspeva. Zaokupno za ovaj scenario jeste da produžite trajanje tokena za pristup kako biste sprečili da on bude duži tokom sesije korisnika. Dodatne informacije o tome kako to da uradite potražite u temi Konfigurisanje trajanja [tokena](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)koji je Microsoft platforma za identitete.

**Preporučeni dokumenti**

- [Kako da konfigurišete jedinstveno prijavljivanje u aplikaciju Proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML jedinstveno prijavljivanje za aplikacije u primeni aplikacije sa proxy serverom aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Razumevanje i rešavanje Azure Active Directory proxy servera aplikacije CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Rešavanje problema sa konfiguracijama kerberos ograničenog delemena za proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)