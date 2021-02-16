---
title: Omogućavanje uređaja
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
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256984"
---
# <a name="enable-device"></a><span data-ttu-id="89c5e-102">Omogućavanje uređaja</span><span class="sxs-lookup"><span data-stu-id="89c5e-102">Enable Device</span></span>

<span data-ttu-id="89c5e-103">**Omogućavanje uređaja pomoću komande PowerShell**</span><span class="sxs-lookup"><span data-stu-id="89c5e-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="89c5e-104">Uradite sledeće komande:</span><span class="sxs-lookup"><span data-stu-id="89c5e-104">Run the following commands:</span></span>

- <span data-ttu-id="89c5e-105">Da biste dobili objekat uređaja: `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="89c5e-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="89c5e-106">Da biste omogućili uređaj: `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="89c5e-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="89c5e-107">Više informacija o konfigurisanju hibridnog spajanja u upravljanim domenima potražite u članku [Konfigurisanje hibridnog pridruživanja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span><span class="sxs-lookup"><span data-stu-id="89c5e-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
