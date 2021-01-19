---
title: Kontroler domena
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901312"
---
# <a name="domain-controller"></a><span data-ttu-id="45a02-102">Kontroler domena</span><span class="sxs-lookup"><span data-stu-id="45a02-102">Domain controller</span></span>

<span data-ttu-id="45a02-103">**Nije moguće omogućiti AAD-DS ili primenu nije uspeo**</span><span class="sxs-lookup"><span data-stu-id="45a02-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="45a02-104">Da biste rešili problem usluge Azure AD Domain (AAD-DS) nije omogućeno ili nije primenjeno, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="45a02-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="45a02-105">Ako koristite postojeću virtuelnu mrežu, potvrdite NSG za pravila koja blokiraju portove neophodne za sinhronizovanje u AAD-DS-u na portalu https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="45a02-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="45a02-106">Potvrdite izbor u polju za proveru da li se u ovom vodiču za rešavanje problema javlja odgovor na vašu grešku  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="45a02-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="45a02-107">Isprobajte usluge Azure A.D. domena u novoj virtualnoj mreži.</span><span class="sxs-lookup"><span data-stu-id="45a02-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="45a02-108">Izvršite Vodič za prvi koraci kako biste primenili AAD-DS, koji je dostupan u [uputstvu da biste kreirali Azure AD Domain usluge domena](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="45a02-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="45a02-109">Ako imate problema sa primenom Azure AD Domain usluge domena, pogledajte članak [Rešavanje problema sa uslugom AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) da biste rešili uobičajene greške koje vam pomažu da ponovo rešite stvari.</span><span class="sxs-lookup"><span data-stu-id="45a02-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="45a02-110">**Nije moguće onemogućiti AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="45a02-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="45a02-111">AAD-DS ne može da se pauzira.</span><span class="sxs-lookup"><span data-stu-id="45a02-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="45a02-112">Ako želite da prestanete da koristite kontrolisano domen, on mora biti izbrisan.</span><span class="sxs-lookup"><span data-stu-id="45a02-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="45a02-113">Ako naiđete na probleme, da biste rešili uobičajene poruke o greškama i povezane korake za rešavanje problema, pogledajte članak [Rešavanje problema sa uslugom Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="45a02-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
