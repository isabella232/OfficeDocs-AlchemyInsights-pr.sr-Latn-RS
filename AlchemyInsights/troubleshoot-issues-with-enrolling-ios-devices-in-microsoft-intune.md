---
title: Rešavanje problema sa upisivanju iOS uređaja u aplikaciju Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823477"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="3c50d-102">Rešavanje problema sa upisivanju iOS uređaja u aplikaciju Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3c50d-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="3c50d-103">Pregledajte resurse navedene ispod da biste odmah rešili problem.</span><span class="sxs-lookup"><span data-stu-id="3c50d-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="3c50d-104">Neke uobičajene poruke o grešci i koraci za rešavanje problema:</span><span class="sxs-lookup"><span data-stu-id="3c50d-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="3c50d-105">**Dostignuto je capava uređaja** Korisnik je upisan više uređaja nego što je ograničenje uređaja.</span><span class="sxs-lookup"><span data-stu-id="3c50d-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3c50d-106">Pregledajte ove dokumente da [biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) [ili promenili ograničenje uređaja.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="3c50d-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="3c50d-107">**Ova usluga nije podržana. Nema smernica za unošenje:** Apple usluga push obaveštenja (APNS) treba da se konfiguriše ili obnovi.</span><span class="sxs-lookup"><span data-stu-id="3c50d-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="3c50d-108">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) da biste pregledali uputstva kako da to uradite.</span><span class="sxs-lookup"><span data-stu-id="3c50d-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="3c50d-109">**Tip korisničke licence nevažeći ili korisničko ime nije prepoznato:** Korisniku mora da bude dodeljena Intune ili EMS licenca.</span><span class="sxs-lookup"><span data-stu-id="3c50d-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="3c50d-110">Pregledajte ove dokumente da biste dodelili licencu preko: [Office centra za administarcije](https://docs.microsoft.com/intune/licenses-assign) ili [Azure portala.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="3c50d-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="3c50d-111">Dodatni resursi koji vam pomažu da rešite problem:</span><span class="sxs-lookup"><span data-stu-id="3c50d-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3c50d-112">Koristite [Intune portal za rešavanje problema da](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) biste dijagnostikovali i rešili uobičajene greške u vezi sa unošenjem.</span><span class="sxs-lookup"><span data-stu-id="3c50d-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3c50d-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="3c50d-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="3c50d-114">Pregledajte ove dokumente da biste videli listu uobičajenih grešaka koje sprečavaju unošenje i rešenja za svaki [od](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) njih: Vodič za rešavanje problema i dokument za [rešavanje problema.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="3c50d-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="3c50d-115">[Saznajte kako da uredite iOS uređaje u aplikaciji Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="3c50d-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

