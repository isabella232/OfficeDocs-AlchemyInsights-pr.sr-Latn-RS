---
title: Rešavanje problema sa ugrađenim Windows uređajima u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708904"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="6d8f3-102">Rešavanje problema sa ugrađenim Windows uređajima u Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6d8f3-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="6d8f3-103">Pregledajte resurse navedene ispod da biste odmah rešili problem.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="6d8f3-104">Neke uobičajene poruke o greškama i korake rezolucije:</span><span class="sxs-lookup"><span data-stu-id="6d8f3-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="6d8f3-105">**Nije moguće instalirati softver, 0x80cf4017:** Certifikat naloga je istekao.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="6d8f3-106">Ponovo preuzmite softver klijenta klijenta u konzoli administracije Intune.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="6d8f3-107">Pregledajte ovu dokumentaciju za više informacija.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="6d8f3-108">**Kôd greške 0x801c0003:** Greška može da se pojavi u sledećim slučajevima:</span><span class="sxs-lookup"><span data-stu-id="6d8f3-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="6d8f3-109">Korisnik ima više uređaja upisano od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="6d8f3-110">Pregledajte ove dokumente da [biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="6d8f3-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="6d8f3-111">"Korisnici mogu da pridruže uređajima na Azure AD" podešeno je na "nijedno".</span><span class="sxs-lookup"><span data-stu-id="6d8f3-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="6d8f3-112">Postavljanje na sve ili izbor korisnika.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-112">Set it to all or select users.</span></span> <span data-ttu-id="6d8f3-113">Pregledajte [ovu dokumentaciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="6d8f3-114">Uređaj je već upisan od strane drugog korisnika.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="6d8f3-115">Ako je to slučaj, uklonite uređaj iz Azure Intune konzole ili ručno opozovite uređaj pre nego što pokušate ponovo.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="6d8f3-116">Uređaj je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="6d8f3-117">Samo Windows 10 pro, obrazovanje i Enterprise MJ mogu da se pridruže Azure aktivnom direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="6d8f3-118">Dodatni resursi koji će vam pomoći da rešite problem:</span><span class="sxs-lookup"><span data-stu-id="6d8f3-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="6d8f3-119">Koristite [portal za rešavanje problema sa Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnostikovali i rešili uobičajene greške unosa.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="6d8f3-120">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="6d8f3-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="6d8f3-121">Redigujte ove dokumente za listu uobičajenih grešaka koje mogu da se prijave i rešenja za svaki: [Vodič za rešavanje problema](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Rešavanje problema sa doktorom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="6d8f3-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="6d8f3-122">[Saznajte kako da Upisite Windows uređaje u Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="6d8f3-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
