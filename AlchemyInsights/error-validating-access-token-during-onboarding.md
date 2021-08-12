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
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946629"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Greška "Došlo je do greške prilikom provere valjanosti tokena za pristup" u toku ankete na radnoj površini

Ova greška se obično posmatra kada token potvrde identiteta istekne. Osvežavanje stranice obično osvežava token. Međutim, ovaj problem može da potraje ako postoje neke smernice uslovnog pristupa primenjene na nalog koji se koristi za analitiku radne površine. Možete da pregledate Azure AD evidencije prijavljivanja na Azure portalu da biste videli da li ima neuspešnih prijavljivanja za nalog koji se koristi za ulaženje u analitiku radne površine.

Dodatne informacije o uslovnom pristupu potražite u [temi Planiranje primene uslovnog pristupa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)