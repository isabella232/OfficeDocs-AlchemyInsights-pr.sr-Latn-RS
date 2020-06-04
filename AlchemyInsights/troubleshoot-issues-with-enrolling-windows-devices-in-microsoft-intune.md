---
title: Rešavanje problema sa enkotrljnim Windows uređajima u usluzi Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665846"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="44e51-102">Rešavanje problema sa enkotrljnim Windows uređajima u usluzi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="44e51-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="44e51-103">Pregledajte dole navedene resurse da biste odmah rešili problem.</span><span class="sxs-lookup"><span data-stu-id="44e51-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="44e51-104">Neke uobičajene poruke o grešci i koraci rešenja:</span><span class="sxs-lookup"><span data-stu-id="44e51-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="44e51-105">**Softver ne može biti instaliran, 0x80cf4017:** Vaš certifikat naloga je istekao.</span><span class="sxs-lookup"><span data-stu-id="44e51-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="44e51-106">Ponovo preuzmite paket za klijentski softver računara u usluzi Intune admin Console.</span><span class="sxs-lookup"><span data-stu-id="44e51-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="44e51-107">Pregledajte ovu dokumentaciju za više informacija.</span><span class="sxs-lookup"><span data-stu-id="44e51-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="44e51-108">**Kôd greške 0x801c0003:** Do greške može doći u sledećim slučajevima:</span><span class="sxs-lookup"><span data-stu-id="44e51-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="44e51-109">Korisnik je više uređaja upisalo od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="44e51-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="44e51-110">Pregledajte ove dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="44e51-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="44e51-111">"Korisnici se mogu pridružiti uređajima za Azure oglas" podešeni su na "nijedan".</span><span class="sxs-lookup"><span data-stu-id="44e51-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="44e51-112">Postavite ga na sve ili izaberite korisnike.</span><span class="sxs-lookup"><span data-stu-id="44e51-112">Set it to all or select users.</span></span> <span data-ttu-id="44e51-113">Pregledajte [ovu dokumentaciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="44e51-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="44e51-114">Uređaj već upisuje drugi korisnik.</span><span class="sxs-lookup"><span data-stu-id="44e51-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="44e51-115">Ako je to slučaj, uklonite uređaj sa Azure Intune konzole ili ručno deprijavite uređaj pre nego što ponovo pokušate.</span><span class="sxs-lookup"><span data-stu-id="44e51-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="44e51-116">Uređaj je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="44e51-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="44e51-117">Samo Windows 10 pro, obrazovanje i Enterprise SKUs mogu da pristupe Azure aktivnom direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="44e51-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="44e51-118">Dodatni resursi koji vam pomažu da rešite problem:</span><span class="sxs-lookup"><span data-stu-id="44e51-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="44e51-119">Koristite [Intune za rešavanje problema](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste ustanovili i rešili uobičajene greške u uvrštavanju.</span><span class="sxs-lookup"><span data-stu-id="44e51-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="44e51-120">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="44e51-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="44e51-121">Pregledajte ove dokumente da biste dobili listu uobičajenih grešaka koje sprečavaju upis i rešenja za svaki: [Vodič za rešavanje problema](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Rešavanje problema sa programom Doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="44e51-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="44e51-122">[Saznajte kako da prijavite Windows uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="44e51-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
