---
title: Onemogućavanje mrežnog skeniranja
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483007"
---
# <a name="disable-network-scan"></a><span data-ttu-id="de92a-102">Onemogućavanje mrežnog skeniranja</span><span class="sxs-lookup"><span data-stu-id="de92a-102">Disable network scan</span></span>

<span data-ttu-id="de92a-103">Skeniranje deljenih mreža može da utiče na performanse.</span><span class="sxs-lookup"><span data-stu-id="de92a-103">Network share scans may impact performance.</span></span>  <span data-ttu-id="de92a-104">Da biste se uverili da klijent ne skenira Mrežno deljenje/datoteke po podrazumevanoj vrednosti, podesite sledeće postavke u aplikaciji Windows Defender na vrednost **TRUE**:</span><span class="sxs-lookup"><span data-stu-id="de92a-104">To ensure the client does not scan network shares/files by default, configure the following settings in the Windows Defender application to **True**:</span></span>

- <span data-ttu-id="de92a-105">Oneblescanscanningmapperdnet</span><span class="sxs-lookup"><span data-stu-id="de92a-105">DisableScanningMappedNetworkDrivesForFullScan</span></span>
- <span data-ttu-id="de92a-106">Oneblescanscaniningnetdatoteke</span><span class="sxs-lookup"><span data-stu-id="de92a-106">DisableScanningNetworkFiles</span></span>