---
title: Uključivanje NDI tehnologije
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023536"
---
# <a name="turn-on-ndi-technology"></a>Uključivanje NDI tehnologije

Tehnologija NDI zahteva dva koraka da biste ga uključili za korisnika:

1. Adminposte zakupca mora da omogući svojstvo "AllowNDIStreaming" u CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Kada se ova promena već napiši, krajnji korisnik mora da uključi tehnologiju NDI® za određenog klijenta iz fascikle **Postavke > Dozvole**.

Više informacija potražite u [temi Korišćenje tehnologije NDI u Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
