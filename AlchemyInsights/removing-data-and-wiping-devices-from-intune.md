---
title: Uklanjanje podataka i brisanje uređaja iz Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440468"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="2e7bf-102">Uklanjanje podataka i brisanje uređaja iz Intune</span><span class="sxs-lookup"><span data-stu-id="2e7bf-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="2e7bf-103">Uređaj se povlače i udaljene radnje za brisanje uređaja mogu da se koriste za uklanjanje podataka o preduzeću koje upravlja Intune ili za izvođenje fabričke početne vrednosti i vraćanje uređaja na podrazumevane postavke.</span><span class="sxs-lookup"><span data-stu-id="2e7bf-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="2e7bf-104">Prijavite se na Microsoft 365 uređaj za upravljanje uređajem i idite na **uređaje "Uređaji**  >  **All Devices**".</span><span class="sxs-lookup"><span data-stu-id="2e7bf-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="2e7bf-105">Izaberite uređaj koji želite da obrišeš.</span><span class="sxs-lookup"><span data-stu-id="2e7bf-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="2e7bf-106">Izaberite tip udaljene obrisa koji želite da uradite.</span><span class="sxs-lookup"><span data-stu-id="2e7bf-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="2e7bf-107">Penzionisati se brišu samo organizacione informacije, dok se pune maramice vraćaju uređaj na fabričke postavke.</span><span class="sxs-lookup"><span data-stu-id="2e7bf-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="2e7bf-108">Izaberite **da** da biste potvrdili izbor.</span><span class="sxs-lookup"><span data-stu-id="2e7bf-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="2e7bf-109">Dok se brisanje ne završi, status radnje uređaja pokazuje kao da je u stanju da se povuče.</span><span class="sxs-lookup"><span data-stu-id="2e7bf-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="2e7bf-110">Nakon dovršenja radnje, mobilni uređaj više nećete videti na listi upravljanog uređaja.</span><span class="sxs-lookup"><span data-stu-id="2e7bf-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="2e7bf-111">**Belešku** Podaci o preduzeću se ne mogu ukloniti sa uređaja koji su PRIDRUŽENI Azure OGLASU.</span><span class="sxs-lookup"><span data-stu-id="2e7bf-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="2e7bf-112">Za sve detalje o uticaju akcija u penziju i brisanju, uključujući ono što se zadržava i šta je izbrisano, pogledajte odeljak [Uklanjanje uređaja pomoću opcije Obriši, penzionisati ili ručno uklanjanje uređaja](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="2e7bf-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="2e7bf-113">Da biste izbrisali sve podatke sa macOS uređaja, pogledajte odeljak [Brisanje svih podataka sa Makos uređaja](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="2e7bf-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>