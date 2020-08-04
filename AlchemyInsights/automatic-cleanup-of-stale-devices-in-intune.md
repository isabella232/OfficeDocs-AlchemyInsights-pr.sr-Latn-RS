---
title: Automatsko čišćenje zastareli uređaja u Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555732"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="b05d8-102">Automatsko čišćenje zastareli uređaja u Intune</span><span class="sxs-lookup"><span data-stu-id="b05d8-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="b05d8-103">Intune dozvoljava administratoru da konfiguriše vremenski interval između 90 i 270 dana, nakon čega se zastareli uređaji uklanjaju iz usluge.</span><span class="sxs-lookup"><span data-stu-id="b05d8-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="b05d8-104">Ova postavka je široka organizacija i nakon aktiviranja odmah stupa na snagu.</span><span class="sxs-lookup"><span data-stu-id="b05d8-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="b05d8-105">Svi uređaji koji nisu prijavljeni na server Intune za period koji premašuje postavku biće trajno izbrisani.</span><span class="sxs-lookup"><span data-stu-id="b05d8-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="b05d8-106">**Belešku** Samo su objekti MDM uređaja prikladni za ovu radnju čišćenja.</span><span class="sxs-lookup"><span data-stu-id="b05d8-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="b05d8-107">EAS samo objekti uređaja su isključeni.</span><span class="sxs-lookup"><span data-stu-id="b05d8-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="b05d8-108">Za dodatne informacije o tome kada uređaj postaje podesan za brisanje na osnovu postavke čišćenja uređaja i njenog "stanja":</span><span class="sxs-lookup"><span data-stu-id="b05d8-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="b05d8-109">Postavka: **Izbriši uređaje posle poslednjeg datuma provere: da (neka vrednost (N) u navedenim danima)**</span><span class="sxs-lookup"><span data-stu-id="b05d8-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="b05d8-110">Na osnovu vrednosti (N) konfigurisanog u postavci, usluga Intune briše uređaj u navedenim danima nakon što je poslednji put uspešno provjeren.</span><span class="sxs-lookup"><span data-stu-id="b05d8-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="b05d8-111">Postavka: **Izbriši uređaje posle poslednjeg datuma provere: ne**</span><span class="sxs-lookup"><span data-stu-id="b05d8-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="b05d8-112">180 dana nakon isteka certifikata uređaja i ne obnavlja se, uređaj se briše.</span><span class="sxs-lookup"><span data-stu-id="b05d8-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="b05d8-113">**Belešku** U oba slučaja uređaj mora biti uspešno registrovan u usluzi Intune.</span><span class="sxs-lookup"><span data-stu-id="b05d8-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="b05d8-114">Registracija se javlja tokom prvog uređaja koji se odvija uz uslugu Intune.</span><span class="sxs-lookup"><span data-stu-id="b05d8-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="b05d8-115">Ako se uređaj uspešno registruje za Intune i ne postane registrovan, uređaj se briše 270 dana nakon upisa.</span><span class="sxs-lookup"><span data-stu-id="b05d8-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="b05d8-116">(90 dana za označavanje uređaja kao opozvanih, a zatim još 180 dana za brisanje zapisa.)</span><span class="sxs-lookup"><span data-stu-id="b05d8-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="b05d8-117">Nijedan mehanizam trenutno ne postoji u alatki Intune da bi se uspostavio rok važenja certifikacije uređaja za neki dati uređaj.</span><span class="sxs-lookup"><span data-stu-id="b05d8-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>