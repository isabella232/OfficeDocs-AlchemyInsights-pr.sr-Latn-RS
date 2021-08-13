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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966123"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Configuration Manager uređaji nedostaju na portalu

Da bi sinhronizacija uređaja funkcionisala, [obavezne internet krajnje tačke](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) moraju da budu dostupne a internog servera koji hostuje ulogu tačke za povezivanje sa ulogom. Da biste rešili problem sa sinhronizacijom uređaja pregledajte **CMGatewaySyncUploadWorker.log** koji se nalazi u tački za povezivanje sa ulogom.

Saznajte više u članku [Prilaganje zakupca u aplikaciju Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
