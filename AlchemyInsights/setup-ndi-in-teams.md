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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935137"
---
# <a name="turn-on-ndi-technology"></a>Uključivanje NDI tehnologije

NDI tehnologija zahteva dva koraka za uključivanje korisnika:

1. Administrator zakupca mora da omoguće svojstvo "Allowndestreaming" u usluzi ci, Smietingpolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Kada ova promena bude popunjena, krajnji korisnik mora da uključi NDI® tehnologiju za određenu klijentsku **> dozvole**.

Više informacija potražite u članku [Korišćenje NDI tehnologije u Microsoft timovima](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
