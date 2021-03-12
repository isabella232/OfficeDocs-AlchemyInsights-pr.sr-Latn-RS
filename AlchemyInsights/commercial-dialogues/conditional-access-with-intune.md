---
title: Korišćenje uslovnog pristupa sa Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749261"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="1cf8e-102">Korišćenje uslovnog pristupa sa Intune</span><span class="sxs-lookup"><span data-stu-id="1cf8e-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="1cf8e-103">Korišćenje uslovnog pristupa pomoću Intune zahteva 3 koraka:</span><span class="sxs-lookup"><span data-stu-id="1cf8e-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="1cf8e-104">Kreirajte smernice za usaglašenost da biste definisali postavke koje moraju da se ispune da bi se uređaj smatrao usaglašenim. Na primer, uređaj mora da ima PIN od najmanje 6 cifara pre nego što se smatra usaglašenim.</span><span class="sxs-lookup"><span data-stu-id="1cf8e-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="1cf8e-105">Kreiranje uslovne smernice za pristup koja definiše resurse koji se čuvaju i koje uslove treba ispuniti da bi se pristupili te resurse. Na primer, uređaj mora da se usklaji pre pristupanja e-pošti preduzeća.</span><span class="sxs-lookup"><span data-stu-id="1cf8e-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="1cf8e-106">Uverite se da su smernice za usaglašenost i uslovne smernice za pristup usmereni na željene grupe korisnika. To može zahtevati Kreiranje određenih grupa korisnika u usluzi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1cf8e-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="1cf8e-107">Pročitajte više o...</span><span class="sxs-lookup"><span data-stu-id="1cf8e-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
