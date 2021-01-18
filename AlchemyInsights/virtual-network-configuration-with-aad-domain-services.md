---
title: Virtuelna konfiguracija sa uslugama AAD Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885648"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="63e02-102">Virtuelna konfiguracija sa uslugama AAD Domain</span><span class="sxs-lookup"><span data-stu-id="63e02-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="63e02-103">Virtuelna konfiguracija sa uslugama AAD Domain uključuje sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="63e02-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="63e02-104">Proveravanje zdravlja domena na Azure portalu https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="63e02-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="63e02-105">Provera NSG za pravila koja blokiraju portove neophodne za sinhronizaciju u uslugama Azure AD Domain. https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="63e02-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="63e02-106">Uverite se da je virtualna mreža primenjena u istoj Azure oblasti kao i domen Azure AD Domain.</span><span class="sxs-lookup"><span data-stu-id="63e02-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="63e02-107">Obezbeđivanje postojećeg domena sa istim imenom domena dostupnom na virtualnoj mreži.</span><span class="sxs-lookup"><span data-stu-id="63e02-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="63e02-108">Više detalja o dizajnu potražite u članku razmatranje usluge Azure virtuelne mreže za podršku AAD uslugama domena, pogledajte članak [razmatranje virtuelne mreže](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="63e02-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

