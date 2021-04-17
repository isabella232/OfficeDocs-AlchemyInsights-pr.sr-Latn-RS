---
title: Nije moguće podesiti ili prikazati smernice AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826105"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="65368-102">Nije moguće podesiti ili prikazati smernice AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="65368-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="65368-103">Kada pokušate da postavite ili prikažete smernicu AllowSelfServicePurchase, dobijate sledeću poruku o grešci:</span><span class="sxs-lookup"><span data-stu-id="65368-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="65368-104">*HandleError: Nije uspelo preuzimanje smernica proizvoda sa SmernicomId "AllowSelfServicePurchase", ErrorMessage – Osnova veza je zatvorena: Došlo je do neočekivane greške prilikom slanja.*</span><span class="sxs-lookup"><span data-stu-id="65368-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="65368-105">To može da bude zbog starije verzije transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="65368-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="65368-106">Da biste povezali uslugu MSCommerce, morate da koristite TLS 1.2 ili veću.</span><span class="sxs-lookup"><span data-stu-id="65368-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="65368-107">Isprobajte sledeće korake da biste omogućili/postavili TLS protokol na 1.2, verifikujte i pokušajte ponovo.</span><span class="sxs-lookup"><span data-stu-id="65368-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="65368-108">Na PowerShell komandnoj liniji (PS C: unesite sledeću komandu da biste postavili TLS protokol na \) verziju 1.2:</span><span class="sxs-lookup"><span data-stu-id="65368-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="65368-109">Potvrdite TLS protokole koji se koriste uz sledeću komandu:</span><span class="sxs-lookup"><span data-stu-id="65368-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="65368-110">Ponovo, po potrebi, ponovotrite komande Nabavi ili Ažuriraj.</span><span class="sxs-lookup"><span data-stu-id="65368-110">Retry the Get or Update commands as needed.</span></span>

