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
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932183"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rešavanje problema sa isporukom e-pošte za kôd greške 5.7.23

Verifikujte SPF DNS zapis za domen u javno dostupnom kontroloru SPF ili DNS zapisa na vebu.

Potvrdite da Odlazna poruka nije identifikovana kao bezedna pošiljka od strane korporacije Microsoft i da je usmerena kroz prostor za isporuke visokog [rizika.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Poruke u grupama za isporuku visokog rizika neće prođeti SPF provere i zbog toga odredišna organizacija e-pošte neće prihvatiti poruke.

Ako ponovo problem potraje, možda ćete morati da se obratite administratoru hosta pošte kom pokušavate da pošaljete e-poštu. Napravite e-poruku o detaljnoj spoljnoj grešci koja je dostupna u poruci o neiskidanju. Microsoft podrška možda neće moći dodatno da pomogne.
