---
title: Greška tima 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700217"
---
# <a name="4c7-error-in-microsoft-teams"></a>Greška 4c7 u Microsoft timovima

Do ove greške dolazi zato što Microsoft zahteva potvrdu identiteta. Kada primenite usluge usluge za Active Directory (AD FS), potvrda identiteta obrazaca se podrazumevano ne omogućava za intranet. Ako Integrisana Windows potvrda identiteta ne uspe, bićete upitani da se prijavite pomoću potvrde identiteta obrazaca.

Da biste rešili ovaj problem, omogućite proveru identiteta obrazaca tako što ćete koristiti proširenje programskog dodatka AD FS Microsoft Management Console (MMC) na računaru koji ima lokalnu kopiju aktivnog direktorijuma. Da biste to uradili, pratite ove korake: 

1. U oknu za navigaciju potražite smernice za **potvrdu identiteta**.
2. U okviru **Radnje** u oknu detalji izaberite stavku **Uredi globalnu primarnu potvrdu identiteta**.
3. Na kartici **intranet** izaberite stavku **potvrda identiteta obrazaca**.
4. Izaberite stavku **u redu** (ili se **primenjuje**).