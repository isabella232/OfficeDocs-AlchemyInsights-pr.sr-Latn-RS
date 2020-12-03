---
title: Greška u licenciranju krajnjeg zareda
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564867"
---
# <a name="endpoint-dlp-licensing-error"></a>Greška u licenciranju krajnjeg zareda

Kada pokušavate da podesite DEPS krajnje tačke, ako primite sledeću grešku:

`Your organization is missing the licenses required to manage these devices`.

Uverite se da imate jednu od sledećih pretplata ili dodataka:

- Microsoft 365 E5
- Microsoft 365 a5 (EDU)
- Microsoft 365 E5 usaglašenost
- Microsoft 365 a5 usaglašenosti
- Microsoft 365 E5 zaštita i upravljanje informacijama
- Microsoft 365 a5 Information zaštita i upravljanje

> [!NOTE]
> To neće funkcionisati za kombinacije licenci kao što su: Win E5 + O365 E5 + EMS E5. Morate da imate čistu M365 E5 licencu da biste postavili ovu funkciju.

Dodatne informacije o licenciranju sa krajnjim tačkom potražite u članku [Dpp licenciranje krajnje tačke.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
