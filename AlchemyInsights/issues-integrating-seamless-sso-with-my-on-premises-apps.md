---
title: Problemi sa integriranjem besprekornog SSO sa mojim lokalnim aplikacijama
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868722"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemi sa integriranjem besprekornog SSO sa mojim lokalnim aplikacijama

Da biste rešili probleme sa integriranjem savršene SSO sa lokalnim aplikacijama, uradite sledeće:

**Preporučeni koraci**

1. Da biste konfigurisali **lokalnu aplikaciju** za **jedinstveno prijavljivanje kroz proxy server**, pogledajte članak podešavanje [lozinki za jedinstveno prijavljivanje pomoću proxy servera](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Problemi sa proxy** serverom za rešavanje problema: preporučujemo da počnete sa pregledanjem toka problema, [otklanjanja proxy servera aplikacije za proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)server da biste utvrdili da li su proxy server aplikacije ispravno konfigurisani. Ako i dalje imate problema prilikom povezivanja sa aplikacijom, slijedite korake za rešavanje problema u [problemima sa proxy aplikacijom za Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Možete da [identifikujete ALS probleme](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomoću sledećih alatki za otklanjanje grešaka pregledača:
    1. Pokrenite pregledač i potražite Veb aplikaciju.
    1. Pritisnite kombinaciju tastera **F12** da biste doveli konzolu za otklanjanje grešaka.
    1. Pokušajte da reprodukujete transakciju i Pregledajte poruku konzole. Kršenje KORS daje grešku konzole o poreklu.
    1. Neke CORS probleme ne možete da razrešite, na primer kada aplikacija preusmerava na login.microsoftonline.com za potvrdu identiteta, a ističe Access Token. KOROVI poziv je zatim propao. Rešenje za ovaj scenario je da produžite životni vek Token Access, da biste ga sprečili da ističe tokom sesije korisnika. Više informacija o tome kako da to uradite potražite u članku broj ћivota koji je [moguće konfigurisati u Microsoft platformi identiteta](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Preporučeni dokumenti**

- [Kako da konfigurišete jedinstveno prijavljivanje u proxy aplikaciji aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SEML jednokratni prijavljivanje za lokalne aplikacije sa proxy serverom aplikacija](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Razumevanje i rešavanje problema sa Azure Active Directory proxy serverom](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Rešavanje problema sa Kerberos ograničenja delegiranja za proxy proxy server](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)