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
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049322"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 greška u Microsoft Teams

Do ove greške dolazi zato Microsoft Teams zahteva potvrdu identiteta obrazaca. Kada primenite Active Directory usluge za ukidanje (AD FS), potvrda identiteta obrazaca nije podrazumevano omogućena za intranet. Ako Windows integrisana potvrda identiteta ne uspe, biće vam zatraženo da se prijavite pomoću potvrde identiteta obrasca.

Da biste rešili ovaj problem, omogućite potvrdu identiteta obrasca pomoću proširenja konzole AD FS Microsoft Management Console (MMC) na računaru koji ima lokalnu kopiju usluge Active Directory. Da biste to uradio, sledite ove korake: 

1. U oknu za navigaciju potražite smernice **za potvrdu identiteta.**
2. U **okviru Radnje** u oknu sa detaljima, izaberite stavku **Uredi globalnu primarnu potvrdu identiteta.**
3. Na kartici **Intranet** izaberite stavku **Potvrda identiteta obrazaca**.
4. Izaberite **stavku U** redu (ili **Primeni**).