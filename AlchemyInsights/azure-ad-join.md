---
title: Azure Active Directory pridruživanje
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405674"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="e6bb6-102">Azure Active Directory pridruživanje</span><span class="sxs-lookup"><span data-stu-id="e6bb6-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="e6bb6-103">Ako po prvi put postavljate registracije uređaja, proverite da li ste pregledali Uvod u upravljanje uređajima u [Azure Active Directory](/azure/active-directory/devices/overview) koji će vas voditi kroz to kako da nabavite uređaje pod kontrolom za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e6bb6-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="e6bb6-104">Ako direktno registrujete uređaje u uslugu Azure AD i upisujete ih u [Intune,](/mem/intune/enrollment/device-enrollment) morate [](/mem/intune/fundamentals/licenses-assign) da se uverite da ste konfigurisali Intune i da prvo imate licenciranje na mestu.</span><span class="sxs-lookup"><span data-stu-id="e6bb6-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="e6bb6-105">Uverite se da ste ovlašćeni za izvršavanje operacija u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e6bb6-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="e6bb6-106">Samo globalni administrator u Azure AD-u može da upravlja postavkama za registracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="e6bb6-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="e6bb6-107">Da biste primenu Azure AD pridruživanja primenili, pogledajte [plan Azure AD Join.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="e6bb6-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="e6bb6-108">Više detalja o rešavanju uobičajenih problema sa Azure AD pridruživanjem možete da vidite u članku Najčešća pitanja za [Azure Ad Join](/azure/active-directory/devices/faq) i za Windows 10 Pro uređaj u članku Nije moguće pridružiti Windows 10 Pro računarU [Azure AD](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)– treba da izvršite nadogradnju na Microsoft zajednicu.</span><span class="sxs-lookup"><span data-stu-id="e6bb6-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
