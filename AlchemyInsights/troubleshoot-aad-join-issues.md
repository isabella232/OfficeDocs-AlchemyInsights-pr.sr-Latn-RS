---
title: Rešavanje problema sa Azure AD pridruživanjem
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
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405759"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="81ec4-102">Rešavanje problema sa Azure AD pridruživanjem</span><span class="sxs-lookup"><span data-stu-id="81ec4-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="81ec4-103">Ako po prvi put postavljate registracije uređaja, proverite da li ste pregledali Uvod u upravljanje uređajima u [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) koji će vas voditi kroz to kako da nabavite uređaje pod kontrolom za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="81ec4-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="81ec4-104">Ako direktno registrujete uređaje u uslugu Azure AD i upisujete ih u [Intune,](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) morate [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) da se uverite da ste konfigurisali Intune i da prvo imate licenciranje na mestu.</span><span class="sxs-lookup"><span data-stu-id="81ec4-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="81ec4-105">Uverite se da ste ovlašćeni za izvršavanje operacija u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="81ec4-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="81ec4-106">Samo globalni administrator u Azure AD-u može da upravlja postavkama za registracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="81ec4-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="81ec4-107">Da biste primenu Azure AD pridruživanja primenili, pogledajte [plan Azure AD Join.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="81ec4-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="81ec4-108">Za više detalja o rešavanju uobičajenih problema sa Azure AD pridruživanjem pogledajte najčešća pitanja o [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) i za Windows 10 Pro uređaj, pogledajte članak Nije moguće pridružiti Windows 10 Pro računarU [Azure AD –](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) treba da izvršite nadogradnju na Microsoft zajednicu</span><span class="sxs-lookup"><span data-stu-id="81ec4-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
