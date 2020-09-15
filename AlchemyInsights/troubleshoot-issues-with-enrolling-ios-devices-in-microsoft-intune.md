---
title: Rešavanje problema sa enrolling iOS uređajima u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669262"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="1d6ac-102">Rešavanje problema sa enrolling iOS uređajima u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1d6ac-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="1d6ac-103">Pregledajte resurse navedene ispod da biste odmah rešili problem.</span><span class="sxs-lookup"><span data-stu-id="1d6ac-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="1d6ac-104">Neke uobičajene poruke o greškama i korake rezolucije:</span><span class="sxs-lookup"><span data-stu-id="1d6ac-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="1d6ac-105">**Vrh uređaja je dostigao** Korisnik ima više uređaja upisano od ograničenja uređaja.</span><span class="sxs-lookup"><span data-stu-id="1d6ac-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="1d6ac-106">Pregledajte ove dokumente da [biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="1d6ac-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="1d6ac-107">**Ova usluga nije podržana. Nema smernica** za prijavljivanje: Apple usluga push obaveštenja (APNS) mora da se konfiguriše ili obnovi.</span><span class="sxs-lookup"><span data-stu-id="1d6ac-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="1d6ac-108">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za uputstva o tome kako to da uradite.</span><span class="sxs-lookup"><span data-stu-id="1d6ac-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="1d6ac-109">**Tip licenciranja korisnika je nevažeći ili nije prepoznat:** Korisniku treba da se dodeli Intune ili EMS licenca.</span><span class="sxs-lookup"><span data-stu-id="1d6ac-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="1d6ac-110">Pregledajte ove dokumente da biste dodelili licencu putem: [Office administracije centra](https://docs.microsoft.com/intune/licenses-assign) ili [Azure portala](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="1d6ac-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="1d6ac-111">Dodatni resursi koji će vam pomoći da rešite problem:</span><span class="sxs-lookup"><span data-stu-id="1d6ac-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1d6ac-112">Koristite [portal za rešavanje problema sa Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnostikovali i rešili uobičajene greške unosa.</span><span class="sxs-lookup"><span data-stu-id="1d6ac-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1d6ac-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="1d6ac-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="1d6ac-114">Redigujte ove dokumente za listu uobičajenih grešaka koje mogu da se prijave i rešenja za svaki: [Vodič za rešavanje problema](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Rešavanje problema sa doktorom](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="1d6ac-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="1d6ac-115">[Saznajte kako da Upisite iOS uređaje u Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="1d6ac-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

