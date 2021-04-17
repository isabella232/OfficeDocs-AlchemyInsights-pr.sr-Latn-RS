---
title: Rešavanje problema sa savetom za bezbednost za provere otkrivanja prevara
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834745"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="fadbb-102">Rešavanje problema sa savetom za bezbednost za provere otkrivanja prevara</span><span class="sxs-lookup"><span data-stu-id="fadbb-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="fadbb-103">Ako dobijate bezbednosni savet u kome piše "Pošiljalac nije uspeo da proveri otkrivanje prevare i možda nije onaj ko izgleda kao da jeste", pošiljalac nije uspeo da prosledi DKIM ili SPF provere identiteta.</span><span class="sxs-lookup"><span data-stu-id="fadbb-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="fadbb-104">Najbolji metod da to rešite jeste da pošiljalac ovlasti sebe.</span><span class="sxs-lookup"><span data-stu-id="fadbb-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="fadbb-105">Ako pošiljalac šalje u vaše ime, morate da ga ovlastite tako što ćete dodati IP adresu pošiljaoca u SPF zapis.</span><span class="sxs-lookup"><span data-stu-id="fadbb-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="fadbb-106">Više [informacija potražite u članku Rešavanje problema sa crvenom (sumnjivom)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) bezbednosnom savetom za provere otkrivanja prevare.</span><span class="sxs-lookup"><span data-stu-id="fadbb-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="fadbb-107">Evo još nekih veza koje vam mogu pomoći:</span><span class="sxs-lookup"><span data-stu-id="fadbb-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="fadbb-108">Kako Microsoft koristi spominjanje smernica za pošiljaoca (SPF) za sprečavanje predstavljanja</span><span class="sxs-lookup"><span data-stu-id="fadbb-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="fadbb-109">Podešavanje spF-a da biste sprečili da se šalju iskažu</span><span class="sxs-lookup"><span data-stu-id="fadbb-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
