---
title: Teams 4c7 greška
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786683"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 greška u aplikaciji Microsoft Teams

Do ove greške dolazi zato što Microsoft Teams zahteva potvrdu identiteta obrasca. Kada primenite Active Directory usluge za ukidanje (AD FS), potvrda identiteta obrazaca nije podrazumevano omogućena za intranet. Ako Windows integrisana potvrda identiteta ne uspe, bićete upitani da se prijavite pomoću potvrde identiteta obrasca.

Da biste rešili ovaj problem, omogućite potvrdu identiteta obrasca pomoću proširenja konzole AD FS Microsoft Management Console (MMC) na računaru koji ima lokalnu kopiju usluge Active Directory. Da biste to uradio, sledite ove korake: 

1. U oknu za navigaciju potražite smernice **za potvrdu identiteta.**
2. U **okviru Radnje** u oknu sa detaljima, izaberite stavku **Uredi globalnu primarnu potvrdu identiteta.**
3. Na kartici **Intranet** izaberite stavku **Potvrda identiteta obrazaca**.
4. Izaberite **stavku U** redu (ili **Primeni**).