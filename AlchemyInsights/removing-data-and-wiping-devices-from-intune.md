---
title: Uklanjanje podataka i brisanje uređaja iz usluge Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416327"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="0ac5b-102">Uklanjanje podataka i brisanje uređaja iz usluge Intune</span><span class="sxs-lookup"><span data-stu-id="0ac5b-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="0ac5b-103">Udaljene radnje „Uklanjanje uređaja“ i „Brisanje uređaja“ mogu se koristiti za uklanjanje podataka preduzeća kojima upravlja Intune ili za vraćanje na fabrička podešavanja i vraćanje uređaja na podrazumevane postavke.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="0ac5b-104">Prijavite se u Microsoft 365 upravljanje uređajima i idite na **Uređaji** > **Svi uređaji**.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="0ac5b-105">Izaberite uređaj koji želite da izbrišete.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="0ac5b-106">Izaberite tip daljinskog brisanja koje želite da izvršite.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="0ac5b-107">Poništavanje briše samo organizacione informacije, dok se potpunim brisanjem uređaj vraća na fabrička podešavanja.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="0ac5b-108">Kliknite na dugme **Da** kako biste potvrdili.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="0ac5b-109">Dok se brisanje ne završi, status radnje uređaja prikazuje se kao *Povlačenje na čekanju*.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="0ac5b-110">Kada se radnja dovrši, više nećete videti mobilni uređaj na listi upravljanih uređaja.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="0ac5b-111">Podaci preduzeća ne mogu se ukloniti sa uređaja PRIDRUŽENIH za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0ac5b-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="0ac5b-112">Za sve detalje o efektu radnji povlačenja i brisanja, uključujući ono što se zadržava i šta se briše, pogledajte sledeću dokumentaciju:</span><span class="sxs-lookup"><span data-stu-id="0ac5b-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="0ac5b-113">[Uklonite uređaje brisanjem, povlačenjem ili ručnim odjavljivanjem uređaja.](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="0ac5b-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="0ac5b-114">Kako obrisati samo korporativne podatke iz aplikacija kojima upravlja Intune</span><span class="sxs-lookup"><span data-stu-id="0ac5b-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="0ac5b-115">[Izbrišite sve podatke sa macOS uređaja](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="0ac5b-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>