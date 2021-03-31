---
title: Rešavanje problema sa hibridnim pridruživanjem u usluzi Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401921"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="cff94-102">Rešavanje problema sa hibridnim pridruživanjem u usluzi Azure AD</span><span class="sxs-lookup"><span data-stu-id="cff94-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="cff94-103">Preporučuje se da se pobrinete da uređaj može da pristupi krajnjim tačkama registracije uređaja u okviru sistemskog naloga koristeći [skriptu za test povezivanja registracije uređaja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="cff94-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="cff94-104">Ako prvi put podešavate registracije uređaja, obavezno pregledajte [Uvod u upravljanje uređajima u usluzi Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) da biste saznali kako da stavite uređaje pod kontrolu usluge Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cff94-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="cff94-105">Ako registrujete uređaje direktno u Azure AD i upišete ih u Intune, najpre se uverite da ste [konfigurisali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i da je [licenciranje](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) spremno.</span><span class="sxs-lookup"><span data-stu-id="cff94-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="cff94-106">Uverite se da ste ovlašćeni za izvršavanje operacija u usluzi Azure AD i lokalnom AD.</span><span class="sxs-lookup"><span data-stu-id="cff94-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="cff94-107">Postavkama za registracije uređaja može da upravlja samo globalni administrator u usluzi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cff94-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="cff94-108">Pored toga, ako podešavate automatske registracije u lokalnom aktivnom direktorijumu, moraćete da budete administrator za aktivni direktorijum i AD FS (ako je primenljivo).</span><span class="sxs-lookup"><span data-stu-id="cff94-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="cff94-109">Za više detalja o rešavanju potencijalnih problema sa hibridnim pridruživanjem, pogledajte [Rešavanje problema sa hibridnim pridruživanjem](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) za podešavanje hibridnih uređaja pridruženih putem usluge Azure AD i upravljanje uređajima pomoću Azure AD portala, pogledajte [Podešavanje hibridnih uređaja pridruženih putem usluge Azure AD (lokalnih uređaja pridruženih u domenu)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) i [Upravljanje uređajima putem Azure portala](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="cff94-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="cff94-110">Da biste rešili uobičajene probleme sa hibridnim pridruživanjem putem usluge Azure Active Directory (AD), pogledajte [Najčešća pitanja u vezi sa hibridnim pridruživanjem putem usluge Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="cff94-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
