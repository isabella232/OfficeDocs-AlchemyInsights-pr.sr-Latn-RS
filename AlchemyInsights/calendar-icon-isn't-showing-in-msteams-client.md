---
title: Ikona kalendara se ne prikazuje u Microsoft klijentu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583925"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Ikona kalendara se ne prikazuje u Microsoft klijentu

Kartica **Kalendar** u timovima zahteva pristup Exchange poštanskom sandučetu putem usluge Exchange Web Services. Exchange poštansko sanduče može biti na mreži ili lokalno. Za korisnike na mreži koji ne vide karticu **Kalendar** , uverite se da su [licencirani za Exchange online poštansko sanduče i da je poštansko sanduče omogućeno](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Ako su vaši korisnici na lokalnom prostoru, morate da potvrdite da je vaša hibridna konfiguracija zdrava. Koristite [Čarobnjak za hibridnu konfiguraciju](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) da biste rešili problem. Imajte u vidu da [Teams zahteva Exchange 2016 CU3 ili noviju verziju](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Više informacija i koraka za rešavanje problema potražite u članku [Rešavanje problema sa Microsoft timovima i interakcijom sistema Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
