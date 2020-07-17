---
title: Uslovni pristup sa Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931450"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="02d60-102">Uslovni pristup sa Intune</span><span class="sxs-lookup"><span data-stu-id="02d60-102">Conditional Access with Intune</span></span>

<span data-ttu-id="02d60-103">Korišćenje **uslovnog pristupa** sa Intune zahteva 3 koraka:</span><span class="sxs-lookup"><span data-stu-id="02d60-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="02d60-104">Kreirajte **smernice usaglašenosti** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) da biste definisali postavke koje moraju da se ispune pre nego što se taj uređaj smatra usaglašen.</span><span class="sxs-lookup"><span data-stu-id="02d60-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="02d60-105">Na primer, uređaj mora da ima PIN kôd od najmanje 6 cifara pre nego što se smatra usaglašen.</span><span class="sxs-lookup"><span data-stu-id="02d60-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="02d60-106">Kreirajte **smernice za uslovno pristup** koje određuju koji resursi se štite i koji uslovi treba da budu ispunjeni da bi pristupili tim resursima.</span><span class="sxs-lookup"><span data-stu-id="02d60-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="02d60-107">[Na primer,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) uređaj mora biti usaglašen sa pristupom korporativnoj e-pošti.</span><span class="sxs-lookup"><span data-stu-id="02d60-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="02d60-108">Uverite se da su **smernice za usaglašavanje** i **smernice uslovnog pristupa** usmerene na željene grupe korisnika.</span><span class="sxs-lookup"><span data-stu-id="02d60-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="02d60-109">Ovo može zahtevati Kreiranje određenih grupa korisnika u Azure aktivnom direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="02d60-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="02d60-110">**Korisni linkovi:**</span><span class="sxs-lookup"><span data-stu-id="02d60-110">**Helpful links:**</span></span>

[<span data-ttu-id="02d60-111">Pregled usaglašenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="02d60-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="02d60-112">Rešavanje problema CA</span><span class="sxs-lookup"><span data-stu-id="02d60-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="02d60-113">Smernice za rešavanje problema</span><span class="sxs-lookup"><span data-stu-id="02d60-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="02d60-114">Da biste zaštitili e-poštu (Exchange online) iz programa Access pomoću uređaja koji nisu usaglašeni, oba dokumenta moraju biti praćena:</span><span class="sxs-lookup"><span data-stu-id="02d60-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="02d60-115">Zaštita pristupa e-pošti sa uređaja pomoću EAS</span><span class="sxs-lookup"><span data-stu-id="02d60-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="02d60-116">Zaštita pristupa e-pošti sa uređaja pomoću savremenih klijenata za potvrdu identiteta kao što je Outlook</span><span class="sxs-lookup"><span data-stu-id="02d60-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)