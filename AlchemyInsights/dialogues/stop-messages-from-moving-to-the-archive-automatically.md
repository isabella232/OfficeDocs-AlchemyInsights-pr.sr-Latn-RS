---
title: Automatsko zaustavljanje premeštanja poruka u arhivu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527114"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="bd0f2-102">Automatsko zaustavljanje premeštanja poruka u arhivu</span><span class="sxs-lookup"><span data-stu-id="bd0f2-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="bd0f2-103">Ako koristite smernice za zadržavanje, možete da promenite starosnu vrednost za zadržavanje u toj politici da biste sprečili automatsko arhiviranje poruka.</span><span class="sxs-lookup"><span data-stu-id="bd0f2-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="bd0f2-104">Evo kako:</span><span class="sxs-lookup"><span data-stu-id="bd0f2-104">Here's how:</span></span>

1. <span data-ttu-id="bd0f2-105">U [Exchange centru administracije](https://go.microsoft.com/fwlink/?linkid=2059104)odaberite oznake za zadržavanje **upravljanja usaglašenosti**  >  .</span><span class="sxs-lookup"><span data-stu-id="bd0f2-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="bd0f2-106">Pronađite Premeštanje za arhiviranje oznake za zadržavanje.</span><span class="sxs-lookup"><span data-stu-id="bd0f2-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="bd0f2-107">U oznakama za zadržavanje promenite period zadržavanja (period arhiviranja) da **nikada ne** sprečite da se stavke automatski arhiviraju pomoću smernica za zadržavanje.</span><span class="sxs-lookup"><span data-stu-id="bd0f2-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="bd0f2-108">To će promeniti postavku arhive za sve Poštanske sandučiće sa ovom oznakom zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="bd0f2-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
