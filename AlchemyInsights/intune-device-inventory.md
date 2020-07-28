---
title: Intune na zalihama uređaja
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440475"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="e1bd9-102">Intune na zalihama uređaja</span><span class="sxs-lookup"><span data-stu-id="e1bd9-102">Intune Device Inventory</span></span>

<span data-ttu-id="e1bd9-103">Uređaj Blade obezbeđuje administratorsku uvid u uređaje pod upravom u usluzi Intune na osnovu uređaja.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="e1bd9-104">Prikazane informacije uključuju: hardver, otkrivene aplikacije, stanje usaglašenosti uređaja i stanje konfiguracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="e1bd9-105">Podaci o zalihama za hardverske i otkrivene aplikacije prikupljaju se u sedmodnevnom ciklusu.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="e1bd9-106">Aplikacije i specifični elementi hardvera su se razlikovale u zavisnosti od operativnog sistema uređaja, kao i od toga da li je uređaj lično ili u vlasništvu preduzeća.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="e1bd9-107">Za više informacija pogledajte odeljak [pregled informacija o uređaju u usluzi Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="e1bd9-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="e1bd9-108">**NAJČEŠĆA PITANJA**</span><span class="sxs-lookup"><span data-stu-id="e1bd9-108">**FAQ**</span></span>

<span data-ttu-id="e1bd9-109">Q: Neću primati popis aplikacija prisutnih na Intune-upisan Windows uređaje.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="e1bd9-110">Zašto da ne?</span><span class="sxs-lookup"><span data-stu-id="e1bd9-110">Why not?</span></span>

<span data-ttu-id="e1bd9-111">A: u ovom trenutku su samo moderne aplikacije navedene za Windows 10 računare koji su identifikovani kao korporativni uređaji.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="e1bd9-112">Intune ne prikuplja informacije o Win32 aplikacijama instaliranim na ovim uređajima.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="e1bd9-113">Q: Zašto se brojevi telefona ne prikupljaju sa svih uređaja?</span><span class="sxs-lookup"><span data-stu-id="e1bd9-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="e1bd9-114">A: telefoni kategorizovani kao korporativni uređaji u Intune nisu identifikovani sa punim telefonskim brojem kada, na primer, pokrećete izveštaj o zalihama za mobilni uređaj.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="e1bd9-115">Brojevi telefona na vašem uređaju su uvek delimično maskirani sa zvezdicom (\* \* \* \*) i prikazuju samo poslednje četiri cifre.</span><span class="sxs-lookup"><span data-stu-id="e1bd9-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>