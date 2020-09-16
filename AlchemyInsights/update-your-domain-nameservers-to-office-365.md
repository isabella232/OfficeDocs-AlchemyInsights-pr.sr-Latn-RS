---
title: Ažurirajte servere imena domena tako da ukazuju na Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734925"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="77aee-102">Ažurirajte servere imena domena tako da ukazuju na Microsoft</span><span class="sxs-lookup"><span data-stu-id="77aee-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="77aee-103">Napomena: Promena servera imena ponekad može da potraje do 48 časova.</span><span class="sxs-lookup"><span data-stu-id="77aee-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="77aee-104">Da biste podesili domen pomoću korporacije Microsoft, serveri imena u vašem registru treba da se ažuriraju.</span><span class="sxs-lookup"><span data-stu-id="77aee-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="77aee-105">Kreirajte ili uredite zapise servera imena u registru domena.</span><span class="sxs-lookup"><span data-stu-id="77aee-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="77aee-106">Idite na veb sajt registra domena i pronađite oblast gde možete da uredite servere imena.</span><span class="sxs-lookup"><span data-stu-id="77aee-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="77aee-107">Kreirajte ili uredite dva zapisa servera imena tako da se podudaraju sa ovim vrednostima:</span><span class="sxs-lookup"><span data-stu-id="77aee-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="77aee-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="77aee-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="77aee-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="77aee-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="77aee-110">Sačuvajte promene.</span><span class="sxs-lookup"><span data-stu-id="77aee-110">Save changes.</span></span>

<span data-ttu-id="77aee-111">Takođe možete da pronađete detaljna uputstva u ovom članku: [Promena servera imena za podešavanje Microsoft 365 sa bilo kojim](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar) registrom domena</span><span class="sxs-lookup"><span data-stu-id="77aee-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  