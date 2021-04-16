---
title: Rešavanje problema sa upisivanju Windows uređaja u aplikaciju Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808985"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="0c215-102">Rešavanje problema sa upisivanju Windows uređaja u aplikaciju Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0c215-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="0c215-103">Pregledajte resurse navedene ispod da biste odmah rešili problem.</span><span class="sxs-lookup"><span data-stu-id="0c215-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="0c215-104">Neke uobičajene poruke o grešci i koraci za rešavanje problema:</span><span class="sxs-lookup"><span data-stu-id="0c215-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="0c215-105">**Softver nije moguće instalirati, a 0x80cf4017:** Certifikat naloga je istekao.</span><span class="sxs-lookup"><span data-stu-id="0c215-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="0c215-106">Ponovo preuzmite softverski paket PC klijenta na Intune kontrolnoj konzoli.</span><span class="sxs-lookup"><span data-stu-id="0c215-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="0c215-107">Pregledajte ovu dokumentaciju za više informacija.</span><span class="sxs-lookup"><span data-stu-id="0c215-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="0c215-108">**Kôd greške 0x801c0003:** Greška može da se pojavi u sledećim scenarijima:</span><span class="sxs-lookup"><span data-stu-id="0c215-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="0c215-109">Korisnik je upisan više uređaja nego što je ograničenje uređaja.</span><span class="sxs-lookup"><span data-stu-id="0c215-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0c215-110">Pregledajte ove dokumente da [biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) [ili promenili ograničenje uređaja.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="0c215-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="0c215-111">"Korisnici mogu da se pridruže uređajima u Azure AD" postavljeno je na "nijedno".</span><span class="sxs-lookup"><span data-stu-id="0c215-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="0c215-112">Podesite na sve korisnike ili ih izaberite.</span><span class="sxs-lookup"><span data-stu-id="0c215-112">Set it to all or select users.</span></span> <span data-ttu-id="0c215-113">Pregledajte [ovu dokumentaciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="0c215-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="0c215-114">Uređaj je već upisao drugi korisnik.</span><span class="sxs-lookup"><span data-stu-id="0c215-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="0c215-115">Ako je to slučaj, uklonite uređaj sa Azure Intune konzole ili ručno uklonite uređaj pre nego što pokušajte ponovo.</span><span class="sxs-lookup"><span data-stu-id="0c215-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="0c215-116">Uređaj je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="0c215-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="0c215-117">Samo Windows 10 Pro, Education i Enterprise SKU-i mogu da se pridruže Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0c215-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="0c215-118">Dodatni resursi koji vam pomažu da rešite problem:</span><span class="sxs-lookup"><span data-stu-id="0c215-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="0c215-119">Koristite [Intune portal za rešavanje problema da](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) biste dijagnostikovali i rešili uobičajene greške u vezi sa unošenjem.</span><span class="sxs-lookup"><span data-stu-id="0c215-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0c215-120">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="0c215-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="0c215-121">Pregledajte ove dokumente da biste videli listu uobičajenih grešaka koje sprečavaju unošenje i rešenja za svaki [od](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) njih: Vodič za rešavanje problema i dokument za [rešavanje problema.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="0c215-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="0c215-122">[Saznajte kako da uredite Windows uređaje u aplikaciji Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="0c215-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
