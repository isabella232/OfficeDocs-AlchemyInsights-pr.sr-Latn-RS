---
title: Status senzora krajnje tačke zaštitnika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676338"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="67030-102">Status senzora krajnje tačke zaštitnika</span><span class="sxs-lookup"><span data-stu-id="67030-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="67030-103">Pločka **Uređaji sa senzorima** se nalazi na sistemsku tablu "Bezbednosne operacije".</span><span class="sxs-lookup"><span data-stu-id="67030-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="67030-104">Ova pločice pruža informacije o mogućnosti pojedinačnog uređaja da pruži senzorske podatke i komunicira sa uslugom "Zaštitnik za krajnju tačku".</span><span class="sxs-lookup"><span data-stu-id="67030-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="67030-105">On prijavljuje koliko uređaja zahteva pažnju i pomaže vam da identifikujete problematične uređaje i preduzmete radnju kako biste rešili poznate probleme.</span><span class="sxs-lookup"><span data-stu-id="67030-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="67030-106">Dva indikatora statusa na pločnici pružaju informacije o broju uređaja koji uslugi ne prijavljujete ispravno:</span><span class="sxs-lookup"><span data-stu-id="67030-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="67030-107">**Pogrešno konfigurisanje** Uređaji koji možda delimično izveštavaju senzorske podatke u uslugu "Zaštitnik za krajnju tačku" i možda imaju greške u konfiguraciji koje treba da se isprave.</span><span class="sxs-lookup"><span data-stu-id="67030-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="67030-108">**Neaktivan** Uređaji koji su prestali da prijavljujeju u uslugu "Zaštitnik za krajnje tačke" više od sedam dana u prošlom mesecu.</span><span class="sxs-lookup"><span data-stu-id="67030-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="67030-109">Klik na bilo koju grupu će vas usmeriti na listu Uređaji filtrirane u skladu sa svojim izborom.</span><span class="sxs-lookup"><span data-stu-id="67030-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="67030-110">Na listi Uređaji možete da filtrirate listu stanja zdravlja prema sledećem statusu:</span><span class="sxs-lookup"><span data-stu-id="67030-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="67030-111">**Aktivno** Uređaji koji aktivno izveštavaju o usluzi "Zaštitnik za krajnju tačku".</span><span class="sxs-lookup"><span data-stu-id="67030-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="67030-112">**Pogrešno konfigurisanje** Uređaji koji možda delimično prijavljujeju podatke senzora u uslugu "Zaštitnik za krajnju tačku", ali imaju greške u konfiguraciji koje treba da se isprave.</span><span class="sxs-lookup"><span data-stu-id="67030-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="67030-113">Pogrešno konfigurisani uređaji mogu imati jedan ili kombinaciju sledećih problema:</span><span class="sxs-lookup"><span data-stu-id="67030-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="67030-114">Nema podataka senzora – Uređaji su prestali da šalju podatke senzora.</span><span class="sxs-lookup"><span data-stu-id="67030-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="67030-115">Ograničena upozorenja se mogu aktivirati sa uređaja.</span><span class="sxs-lookup"><span data-stu-id="67030-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="67030-116">Komunikacija sa otežava – Mogućnost komunikacije sa uređajem je uklonjena.</span><span class="sxs-lookup"><span data-stu-id="67030-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="67030-117">Slanje datoteka radi dubinske analize, blokiranje datoteka, izolacija uređaja od mreže i drugih radnji koje zahtevaju komunikaciju sa uređajem možda neće raditi.</span><span class="sxs-lookup"><span data-stu-id="67030-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="67030-118">**Neaktivan** Uređaji koji su prestali da prijavljujeju izveštavanje u uslugu "Zaštitnik za krajnje tačke".</span><span class="sxs-lookup"><span data-stu-id="67030-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="67030-119">Možete da preuzmete celu listu u CSV formatu pomoću funkcije "Izvoz".</span><span class="sxs-lookup"><span data-stu-id="67030-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="67030-120">Više informacija potražite u članku [Provera stanja zdravstvenog stanja senzora u programu Microsoft zaštitnik za krajnju tačku.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="67030-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="67030-121">Više informacija o tome šta je izazvalo neaktivnost ili neispravno konfigurisanje uređaja potražite u članku Popravka neispravno skeniranih senzora u programu Microsoft zaštitnik za krajnju [tačku.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="67030-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
