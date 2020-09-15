---
title: Rešavanje problema sa savetom za bezbednost za proveru otkrivanja prevara
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658424"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="6366b-102">Rešavanje problema sa savetom za bezbednost za proveru otkrivanja prevara</span><span class="sxs-lookup"><span data-stu-id="6366b-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="6366b-103">Ako dobijate sigurnosnu napojnicu na kojoj piše "Pošiljalac nije uspeo za otkrivanje otkrivanja prevara i možda nije ono što izgleda", pošiljalac nije uspeo da prosledi DKIM ili SPF proveru identiteta.</span><span class="sxs-lookup"><span data-stu-id="6366b-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="6366b-104">Najbolji način da se ovo reši je da pošiljalac sama sebe dozvoli.</span><span class="sxs-lookup"><span data-stu-id="6366b-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="6366b-105">Ako pošiljalac šalje u vaše ime, morate da im dozvolite tako što ćete dodati IP adresu pošiljaoca u SPF zapis.</span><span class="sxs-lookup"><span data-stu-id="6366b-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="6366b-106">Pogledajte članak [Rešavanje problema sa crvenom bojom (sumnjiva) za proveru prevare](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="6366b-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="6366b-107">Evo još neke veze koje vam mogu pomoći:</span><span class="sxs-lookup"><span data-stu-id="6366b-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="6366b-108">Kako Microsoft koristi okvir "smernice za pošiljaoca" (SPF) da bi sprečio lažno pojavljivanje</span><span class="sxs-lookup"><span data-stu-id="6366b-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="6366b-109">Podešavanje SPF tako da sprečite lažno pojavljivanje</span><span class="sxs-lookup"><span data-stu-id="6366b-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
