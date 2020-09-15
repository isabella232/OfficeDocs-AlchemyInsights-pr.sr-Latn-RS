---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717339"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Rešavanje problema sa isporukom e-pošte za kôd greške 5.7.23

Verifikujte program za SPF za vaš domen na javnom dostupnom kontroloru SPF ili DNS zapisima na vebu.

Potvrdite da Microsoft nije identifikovan kao bezvredna poruka i usmeren kroz [visoki prostor za isporuku rizika](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Poruke u bazenu visokog rizika neće proći CIF provere i zato neće biti prihvaćeni od strane odredišta e-pošte.

Ako se problem ponavlja, možda ćete morati da se obratite administratoru domaćina pošte kojem pokušavate da pošaljete e-poruku. Zabeležite detaljnu spoljašnju grešku dostupnu u poruci "iskakanja". Microsoft Support možda neće moći da pomogne dalje.
