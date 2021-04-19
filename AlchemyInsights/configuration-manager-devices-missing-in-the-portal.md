---
title: Configuration Manager uređaji nedostaju na portalu
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
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817258"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Configuration Manager uređaji nedostaju na portalu

Da bi sinhronizacija uređaja funkcionisala, [obavezne internet krajnje tačke](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) moraju da budu dostupne a internog servera koji hostuje ulogu tačke za povezivanje sa ulogom. Da biste rešili problem sa sinhronizacijom uređaja pregledajte **CMGatewaySyncUploadWorker.log** koji se nalazi u tački za povezivanje sa ulogom.

Saznajte više u članku [Prilaganje zakupca u aplikaciju Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
