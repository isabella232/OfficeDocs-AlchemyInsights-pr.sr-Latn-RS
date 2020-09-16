---
title: Nije moguće postavljanje ili prikaz smernice za Allowselfnabavka.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735213"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="4c6a9-102">Nije moguće postavljanje ili prikaz smernice za Allowselfnabavka.</span><span class="sxs-lookup"><span data-stu-id="4c6a9-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="4c6a9-103">Kada pokušate da postavljate ili prikazujete smernice za Allowselfusluge, dobijate sledeću poruku o grešci:</span><span class="sxs-lookup"><span data-stu-id="4c6a9-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="4c6a9-104">*Ruguerror: nije uspelo preuzimanje smernica za proizvode sa šifrom polise "Allowselfservicenabavka", ErrorMessage – osnovna veza je zatvorena: došlo je do neočekivane greške na slanju.*</span><span class="sxs-lookup"><span data-stu-id="4c6a9-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="4c6a9-105">To je možda zbog starije verzije sistema Security Layer (TLS).</span><span class="sxs-lookup"><span data-stu-id="4c6a9-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="4c6a9-106">Da biste povezali MSCommerce uslugu, morate da koristite TLS 1,2 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="4c6a9-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="4c6a9-107">Isprobajte sledeće korake da biste omogućili/odredili TLS protokol u 1,2, Verifikujte i pokušajte ponovo.</span><span class="sxs-lookup"><span data-stu-id="4c6a9-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="4c6a9-108">Na komandnoj liniji PowerShell (PS C: \) Unesite sledeću komandu da biste na verziju 1,2 odredili TLS protokol:</span><span class="sxs-lookup"><span data-stu-id="4c6a9-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="4c6a9-109">Potvrdite TLS protokol u upotrebi sa sledećim komandama:</span><span class="sxs-lookup"><span data-stu-id="4c6a9-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="4c6a9-110">Ponovo pokušajte da izvršite kreiranje ili ažuriranje komandi po potrebi.</span><span class="sxs-lookup"><span data-stu-id="4c6a9-110">Retry the Get or Update commands as needed.</span></span>

