---
title: Rešavanje problema sa upisivanju Android uređaja u aplikaciji Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830956"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="9d731-102">Rešavanje problema sa upisivanju Android uređaja u aplikaciji Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9d731-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="9d731-103">Pregledajte resurse navedene ispod da biste odmah rešili problem.</span><span class="sxs-lookup"><span data-stu-id="9d731-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9d731-104">Neki uobičajeni problemi i koraci za rešavanje problema:</span><span class="sxs-lookup"><span data-stu-id="9d731-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="9d731-105">**Greška "Uređaj nije šifrovan" na portalu preduzeća:** Novije verzije operativnog sistema Android, naročito verzije v7.0, zahtevaju pokreni kod da biste se uverili da je uređaj potpuno šifrovan.</span><span class="sxs-lookup"><span data-stu-id="9d731-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="9d731-106">Uobičajena rešenja su omogućavanje PIN koda za pokretanje ili potpunog šifrovanja uređaja.</span><span class="sxs-lookup"><span data-stu-id="9d731-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="9d731-107">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="9d731-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="9d731-108">Uređaji ne uspevaju da se prijavite pomoću usluge Intune ili da se prikažu kao **"Neispravan" na Intune kontrolnoj konzoli:** Neki Samsung 4.4 i 5.5 uređaji možda neće prijaviti uslugu.</span><span class="sxs-lookup"><span data-stu-id="9d731-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="9d731-109">Postoje 3 moguća rešenja za ovaj problem:</span><span class="sxs-lookup"><span data-stu-id="9d731-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="9d731-110">Ručno otvorite aplikaciju Intune Company Portal, koja će automatski pokrenuti sinhronizaciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="9d731-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="9d731-111">Ažurirajte uređaj na Android 6.0 ili noviju.</span><span class="sxs-lookup"><span data-stu-id="9d731-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="9d731-112">Onemogućite samsung Smart Manager da upravlja intune Company Portalom.</span><span class="sxs-lookup"><span data-stu-id="9d731-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="9d731-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za više detalja o ovim problemima i rešenjima.</span><span class="sxs-lookup"><span data-stu-id="9d731-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="9d731-114">**Greška "Tip korisničke licence** je nevažeći" ili "Nije prepoznato korisničko **ime":** Korisniku treba da bude dodeljena Intune ili EMS licenca.</span><span class="sxs-lookup"><span data-stu-id="9d731-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9d731-115">Pregledajte ove dokumente da biste dodelili licencu preko: Office centra za administarcije ili Azure portala.</span><span class="sxs-lookup"><span data-stu-id="9d731-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="9d731-116">Dodatni resursi koji vam pomažu da rešite problem:</span><span class="sxs-lookup"><span data-stu-id="9d731-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9d731-117">Koristite [Intune portal za rešavanje problema da](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) biste dijagnostikovali i rešili uobičajene greške u vezi sa unošenjem.</span><span class="sxs-lookup"><span data-stu-id="9d731-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9d731-118">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="9d731-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="9d731-119">Pregledajte [ovaj](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) dokument da biste videli listu uobičajenih grešaka koje sprečavaju unošenje i rešenja za svaku od njih.</span><span class="sxs-lookup"><span data-stu-id="9d731-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="9d731-120">[Saznajte kako da uklonite Android uređaje u aplikaciju Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="9d731-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
