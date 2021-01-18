---
title: Konfigurisanje usluge domena
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885689"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="6e828-102">Nije moguće omogućiti AAD-DS ili primenu nije uspeo</span><span class="sxs-lookup"><span data-stu-id="6e828-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="6e828-103">Da biste rešili problem usluge Azure AD Domain (AAD-DS) nije omogućeno ili nije primenjeno, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="6e828-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="6e828-104">Ako koristite postojeću virtuelnu mrežu, potvrdite NSG za pravila koja blokiraju portove neophodne za sinhronizovanje u AAD-DS-u na portalu https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="6e828-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="6e828-105">Potvrdite izbor u polju za proveru da li se u ovom vodiču za rešavanje problema javlja odgovor na vašu grešku  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="6e828-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="6e828-106">Isprobajte usluge Azure A.D. domena u novoj virtualnoj mreži.</span><span class="sxs-lookup"><span data-stu-id="6e828-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="6e828-107">Izvršite Vodič za prvi koraci kako biste primenili AAD-DS: [Kreirajte i konfigurišite usluge AAD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="6e828-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="6e828-108">Ako imate problema sa primenom Azure AD Domain usluge domena, pogledajte članak [Rešavanje problema sa uslugom AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) da biste rešili uobičajene greške koje vam pomažu da ponovo rešite stvari.</span><span class="sxs-lookup"><span data-stu-id="6e828-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="6e828-109">**Nije moguće onemogućiti AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="6e828-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="6e828-110">AAD-DS ne može da se pauzira.</span><span class="sxs-lookup"><span data-stu-id="6e828-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="6e828-111">Ako želite da prestanete da koristite kontrolisano domen, on mora biti izbrisan.</span><span class="sxs-lookup"><span data-stu-id="6e828-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="6e828-112">Da biste izbrisali kontrolisani domen, pogledajte članak [Brisanje usluge AAD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="6e828-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



