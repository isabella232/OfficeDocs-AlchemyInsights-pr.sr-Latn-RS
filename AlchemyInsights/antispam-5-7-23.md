---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821425"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rešavanje problema sa isporukom e-pošte za kôd greške 5.7.23

Verifikujte SPF DNS zapis za domen u javno dostupnom kontroloru SPF ili DNS zapisa na vebu.

Potvrdite da Odlazna poruka nije identifikovana kao bezedna pošiljka od strane korporacije Microsoft i da je usmerena kroz prostor za isporuke visokog [rizika.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Poruke u grupama za isporuku visokog rizika neće prođeti SPF provere i zbog toga odredišna organizacija e-pošte neće prihvatiti poruke.

Ako ponovo problem potraje, možda ćete morati da se obratite administratoru hosta pošte kom pokušavate da pošaljete e-poštu. Napravite e-poruku o detaljnoj spoljnoj grešci koja je dostupna u poruci o neiskidanju. Microsoft podrška možda neće moći dodatno da pomogne.
