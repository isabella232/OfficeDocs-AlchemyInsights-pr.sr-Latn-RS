---
title: Rešavanje problema sa SMTP potvrdom identiteta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826429"
---
# <a name="solving-smtp-authentication-issues"></a>Rešavanje problema sa SMTP potvrdom identiteta

Ako dobijate greške 5.7.57 ili 5.7.3 kada pokušavate da pošaljete SMTP e-poštu i potvrdite identitet kod klijenta ili aplikacije, postoji nekoliko stvari koje bi trebalo da proverite:

- Potvrda identiteta SMTP prosleđivanje može biti onemogućena u zakupca ili u poštanskom sandučetu koje pokušavate da koristite (proverite obe postavke). Da biste pročitali više, pogledajte [omogućavanje ili onemogućavanje SMTP prosleđivanje autorizovanog klijenta.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)

- Proverite da [li su Azure bezbednosne podrazumevane](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) vrednosti omogućene za vašeg zakupca; ako je omogućena, SMTP potvrda identiteta pomoću osnovne potvrde identiteta (poznata i kao zatamnjena; ovo će koristiti korisničko ime i lozinku) neće uspeti.
