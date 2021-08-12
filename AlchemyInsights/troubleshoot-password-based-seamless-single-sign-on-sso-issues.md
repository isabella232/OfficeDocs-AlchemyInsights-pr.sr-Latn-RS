---
title: Rešavanje problema sa nesumnjivim jedinstvenim prijavljivanjem (SSO) zasnovanim na lozinki
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972838"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Rešavanje problema sa nesumnjivim jedinstvenim prijavljivanjem (SSO) zasnovanim na lozinki

Da biste saznali osnove SSO-a zasnovane na lozinki, pogledajte potvrdu identiteta zasnovanu na [lozinki u programu Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Konfigurisanje SSO zasnovanog na lozinki**

1. [Konfigurišite jedinstveno](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) prijavljivanje zasnovano na lozinki – Ovaj članak govori o opciji SSO zasnovanoj na lozinki. Ako aplikacija koju dodajete zahteva prilagođenu konfiguraciju i treba da koristite SSO zasnovan na lozinki, onda je ovaj članak za vas.
2. [Konfigurišite jedinstveno prijavljivanje zasnovano](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) na lozinki za aplikacije premeštenih aplikacija – Proxy aplikacija podržava nekoliko režima jedinstvenog prijavljivanje. Prijavljivanje zasnovano na lozinki namenjeno je aplikacijama koje koriste kombinaciju korisničkog imena/lozinke za potvrdu identiteta. Kada konfigurišete prijavljivanje zasnovano na lozinki za aplikaciju, korisnici moraju jednom da se prijave u primenjenu aplikaciju. Nakon toga, Azure Active Directory skladišti informacije za prijavljivanje i automatski ih pruža aplikaciji kada im korisnici pristupe daljinski.
    - Trebalo bi da ste već objavili i testirali aplikaciju sa proxy serverom aplikacije. Ako to nije moguće, pratite korake u temi Objavljivanje aplikacija pomoću proxyja [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) aplikacije, a zatim nastavite sa konfiguracijom SSO servera zasnovanog na lozinki za aplikacije.

Da biste rešili probleme sa SSO-om zasnovanim na lozinki, pogledajte rešavanje problema sa jedinstvenim prijavljivanjem zasnovanim na [lozinki u Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
