---
title: Uslovno pristup sa Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807673"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="a9686-102">Uslovno pristup sa Intune</span><span class="sxs-lookup"><span data-stu-id="a9686-102">Conditional Access with Intune</span></span>

<span data-ttu-id="a9686-103">Korišćenje  **uslovnog pristupa**  pomoću Intune zahteva 3 koraka:</span><span class="sxs-lookup"><span data-stu-id="a9686-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="a9686-104">Kreirajte  **smernice za usaglašenost**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) da biste definisali postavke koje moraju da se ispune da bi se uređaj smatrao usaglašenim.</span><span class="sxs-lookup"><span data-stu-id="a9686-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="a9686-105">Na primer, uređaj mora da ima PIN od najmanje 6 cifara pre nego što se smatra usaglašenim.</span><span class="sxs-lookup"><span data-stu-id="a9686-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="a9686-106">Kreiranje **uslovne smernice za pristup**  koja definiše resurse koji se čuvaju i koje uslove treba ispuniti da bi se pristupili te resurse.</span><span class="sxs-lookup"><span data-stu-id="a9686-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="a9686-107">[Na primer,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  uređaj mora da se usklaji pre pristupanja e-pošti preduzeća.</span><span class="sxs-lookup"><span data-stu-id="a9686-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="a9686-108">Uverite se da su **smernice za usaglašenost**  i  **uslovne smernice za pristup**  usmereni na željene grupe korisnika.</span><span class="sxs-lookup"><span data-stu-id="a9686-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="a9686-109">To može zahtevati Kreiranje određenih grupa korisnika u usluzi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a9686-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="a9686-110">**Korisne veze:**</span><span class="sxs-lookup"><span data-stu-id="a9686-110">**Helpful links:**</span></span>

[<span data-ttu-id="a9686-111">Pregled usaglašenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="a9686-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="a9686-112">Rešavanje problema sa kom</span><span class="sxs-lookup"><span data-stu-id="a9686-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="a9686-113">Smernice za rešavanje problema</span><span class="sxs-lookup"><span data-stu-id="a9686-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="a9686-114">Da biste zaštitili e-poštu (Exchange online) iz programa Access uređajima koji nisu usaglašeni, oba dokumenta moraju da se slede:</span><span class="sxs-lookup"><span data-stu-id="a9686-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="a9686-115">Zaštita pristupa e-poštom sa uređaja pomoću EAS</span><span class="sxs-lookup"><span data-stu-id="a9686-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="a9686-116">Zaštita pristupa e-poštom sa uređaja pomoću modernih klijenata za potvrdu identiteta kao što je Outlook</span><span class="sxs-lookup"><span data-stu-id="a9686-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)