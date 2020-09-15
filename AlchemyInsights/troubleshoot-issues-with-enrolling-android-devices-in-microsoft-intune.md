---
title: Rešavanje problema sa ugrađenim Android uređajima u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689968"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d03e1-102">Rešavanje problema sa ugrađenim Android uređajima u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d03e1-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d03e1-103">Pregledajte resurse navedene ispod da biste odmah rešili problem.</span><span class="sxs-lookup"><span data-stu-id="d03e1-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d03e1-104">Neke uobičajene korake i korake rezolucije:</span><span class="sxs-lookup"><span data-stu-id="d03e1-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d03e1-105">**Greška uređaja nije šifrovana na portalu preduzeća:** Novije verzije programa android, naročito počevši od programa v 7.0, zahtevaju kôd za pokretanje sistema da biste se uverili da je uređaj potpuno šifrovan.</span><span class="sxs-lookup"><span data-stu-id="d03e1-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d03e1-106">Uobičajena rešenja su da omogućite PIN za pokretanje ili u potpunosti šifrujete uređaj.</span><span class="sxs-lookup"><span data-stu-id="d03e1-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d03e1-107">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="d03e1-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d03e1-108">**Uređaji se ne mogu prijaviti pomoću usluge Intune ili prikazani kao "nezdravi" u konzoli administracije Intune:** Neki Samsung 4,4 i 5,5 uređaji se možda neće prijaviti u uslugu.</span><span class="sxs-lookup"><span data-stu-id="d03e1-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d03e1-109">Postoji 3 moguća rešenja za ovaj problem:</span><span class="sxs-lookup"><span data-stu-id="d03e1-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d03e1-110">Ručno otvorite aplikaciju Intune Company, koja će automatski započeti sinhronizaciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="d03e1-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d03e1-111">Ažurirajte uređaj na Android 6,0 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="d03e1-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d03e1-112">Onemogućavanje Samsung pametnog menadžera iz upravljanja portalu Intune Company.</span><span class="sxs-lookup"><span data-stu-id="d03e1-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d03e1-113">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za dodatne detalje o ovim temama i rezolucijama.</span><span class="sxs-lookup"><span data-stu-id="d03e1-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d03e1-114">**Tip licenciranja korisnika je nevažeći** ili **korisničko ime nisu prepoznati grešku:** korisniku treba da se DODELI Intune ili Ems licenca.</span><span class="sxs-lookup"><span data-stu-id="d03e1-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d03e1-115">Pregledajte ove dokumente da biste dodelili licencu putem: Office administracije centra ili Azure portala.</span><span class="sxs-lookup"><span data-stu-id="d03e1-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d03e1-116">Dodatni resursi koji će vam pomoći da rešite problem:</span><span class="sxs-lookup"><span data-stu-id="d03e1-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d03e1-117">Koristite [portal za rešavanje problema sa Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnostikovali i rešili uobičajene greške unosa.</span><span class="sxs-lookup"><span data-stu-id="d03e1-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d03e1-118">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.</span><span class="sxs-lookup"><span data-stu-id="d03e1-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d03e1-119">Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za listu uobičajenih grešaka koje sprečavaju upis i rezoluciju na svaki.</span><span class="sxs-lookup"><span data-stu-id="d03e1-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d03e1-120">[Saznajte kako da Upisite Android uređaje u Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="d03e1-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
