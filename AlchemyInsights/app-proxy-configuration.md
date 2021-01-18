---
title: Konfiguracija proxy aplikacije
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885526"
---
# <a name="app-proxy-configuration"></a>Konfiguracija proxy aplikacije

1. Da biste razumeli kako da konfigurišete aplikaciju proxy servera u okviru Azure AD da biste izložili lokalne aplikacije u oblaku, pogledajte [članak konfigurisanje proxy aplikacije za aplikaciju](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Jedinstveno prijavljivanje (SSO) omogućava korisnicima da pristupe aplikaciji bez autentične identiteta. Omogućava jedinstvenu potvrdu identiteta koja se pojavljuje u oblaku, protiv Azure aktivnog direktorijuma i omogućava uslugu ili konektor da oponaša korisnika da bi dovršio sve dodatne izazove potvrde identiteta iz aplikacije. Da biste saznali više, pogledajte [članak konfigurisanje jedinstvenog prijavljivanja u proxy aplikaciji aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Koristite [Ovaj članak](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) da biste rešili probleme sa uobičajenim problemima koje osobe suočavaju kada kreiraju novu proxy aplikaciju aplikacije.
4. Ako imate problem sa podešavanjem potvrde identiteta na svoju aplikaciju, možda će biti potrebno da [rešite probleme Kerberos konfiguracije delegiranja u delegaciji aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ili da biste sledili uputstva za [Konfigurisanje aplikacije sa pingbonom](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) da biste rešili problem.
