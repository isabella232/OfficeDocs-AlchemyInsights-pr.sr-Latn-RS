---
title: Došlo je do greške prilikom provere valjanosti tokena za pristup tokom nalaženja anatike radne površine
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813702"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Greška "Došlo je do greške prilikom provere valjanosti tokena za pristup" u toku ankete na radnoj površini

Ova greška se obično posmatra kada token potvrde identiteta istekne. Osvežavanje stranice obično osvežava token. Međutim, ovaj problem može da potraje ako postoje neke smernice uslovnog pristupa primenjene na nalog koji se koristi za analitiku radne površine. Možete da pregledate Azure AD evidencije prijavljivanja na Azure portalu da biste videli da li ima neuspešnih prijavljivanja za nalog koji se koristi za ulaženje u analitiku radne površine.

Dodatne informacije o uslovnom pristupu potražite u [temi Planiranje primene uslovnog pristupa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)