---
title: Uključivanje nadgledanja poštanskog sandučeta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483542"
---
# <a name="turn-on-mailbox-auditing"></a>Uključivanje nadgledanja poštanskog sandučeta

Da biste uključili nadzor poštanskog sandučeta za jednog korisnika ili celu organizaciju, uradite sledeće cmdlet lokacije iz udaljenog PowerShell:

- **Pojedinačni korisnik**: Set-Mailbox-identitet "Džejn Dow" – $TRUE
- **Organizacija**: Get-Mailbox-Rezultsize neograničen-filter {RecipientTypeDetails-EQ "Korisnikopoštansko sanduče"} | Set-Mailbox-Revizoit $true

Da biste saznali više, pogledajte članak [Upravljanje nadgledanjem poštanskog sandučeta](https://go.microsoft.com/fwlink/?linkid=2103668).