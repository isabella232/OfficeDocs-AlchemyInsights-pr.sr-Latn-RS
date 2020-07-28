---
title: Lociranje izgubljenih iOS uređaja sa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440427"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="d19ca-102">Lociranje izgubljenih iOS uređaja sa Intune</span><span class="sxs-lookup"><span data-stu-id="d19ca-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="d19ca-103">Omogućavanje gubitka režima na iOS uređaju omogućava administratoru da na zaključanom ekranu prikaže poruku i broj telefona kontakta.</span><span class="sxs-lookup"><span data-stu-id="d19ca-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="d19ca-104">Kada je izgubljen režim omogućen, administrator može da koristi radnju lociranje uređaja da bi identifikovao fizičku lokaciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="d19ca-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="d19ca-105">Radnja lociranja uređaja u Intune radi sa iOS uređajima da bi prikazala lokaciju određenog uređaja na mapi.</span><span class="sxs-lookup"><span data-stu-id="d19ca-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="d19ca-106">Korišćenje ove radnje zahteva da se iOS uređaj nalazi u:</span><span class="sxs-lookup"><span data-stu-id="d19ca-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="d19ca-107">Nadgledan režim</span><span class="sxs-lookup"><span data-stu-id="d19ca-107">Supervised mode</span></span>
- <span data-ttu-id="d19ca-108">Izgubljeni režim</span><span class="sxs-lookup"><span data-stu-id="d19ca-108">Lost mode</span></span>

<span data-ttu-id="d19ca-109">Više informacija potražite u članku [Omogućavanje izgubljenog režima na iOS/iPadOS uređajima sa Intune](https://docs.microsoft.com/intune/device-lost-mode) i [Lociranje izgubljenih ili ukradenih iOS/Ipados uređaja sa Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="d19ca-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="d19ca-110">**NAJČEŠĆA PITANJA**</span><span class="sxs-lookup"><span data-stu-id="d19ca-110">**FAQ**</span></span>

<span data-ttu-id="d19ca-111">Q: izdao sam udaljenu radnju da biste uklonili podatke o preduzeću sa uređaja, a sada je zaglavljeno u stanju čekanja.</span><span class="sxs-lookup"><span data-stu-id="d19ca-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="d19ca-112">A: da bi se udaljena radnja uspešno dovršila, ciljni uređaj mora biti na mreži i zdrav.</span><span class="sxs-lookup"><span data-stu-id="d19ca-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="d19ca-113">U sledećim situacijama, udaljena radnja ostaje u stanju čekanja 30 dana ili dok uređaj ne bude priznao komandu:</span><span class="sxs-lookup"><span data-stu-id="d19ca-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="d19ca-114">Kada uređaj nema vezu</span><span class="sxs-lookup"><span data-stu-id="d19ca-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="d19ca-115">Kada uređaj izgubi status upravljanja sa Intune</span><span class="sxs-lookup"><span data-stu-id="d19ca-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="d19ca-116">Ako mislite da se uređaj više ne proverava i da neće moći da ukloni podatke o preduzeću, izaberite opciju "Izbriši".</span><span class="sxs-lookup"><span data-stu-id="d19ca-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="d19ca-117">Brisanje uklanja zapis uređaja tako da se više ne pojavljuje na listi za Intune uređaja.</span><span class="sxs-lookup"><span data-stu-id="d19ca-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="d19ca-118">Ako uređaj ponovo postane aktivan, korisnik će morati da je ponovo prijavi.</span><span class="sxs-lookup"><span data-stu-id="d19ca-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="d19ca-119">Q: Zašto određene udaljene radnje nisu dostupne da bi se koristila?</span><span class="sxs-lookup"><span data-stu-id="d19ca-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="d19ca-120">A: ne podržavaju sve platforme sve radnje udaljenog uređaja.</span><span class="sxs-lookup"><span data-stu-id="d19ca-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="d19ca-121">Sledeće udaljene radnje su karakteristične za platformu, tako da su dostupne samo za platforme koje su obeležene.</span><span class="sxs-lookup"><span data-stu-id="d19ca-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="d19ca-122">Zaobiđi zaključavanje aktivacije (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="d19ca-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="d19ca-123">Novi početak (samo za Windows)</span><span class="sxs-lookup"><span data-stu-id="d19ca-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="d19ca-124">Izgubljeni režim (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="d19ca-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="d19ca-125">Lociranje uređaja (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="d19ca-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="d19ca-126">Ponovo pokreni (samo za Windows)</span><span class="sxs-lookup"><span data-stu-id="d19ca-126">Restart (Windows only)</span></span>

<span data-ttu-id="d19ca-127">Više detalja o svakoj radnji potražite u članku [Dostupne radnje uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="d19ca-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>