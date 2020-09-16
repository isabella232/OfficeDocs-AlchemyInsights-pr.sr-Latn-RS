---
title: Intune zalihe uređaja
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667892"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="6c49f-102">Intune zalihe uređaja</span><span class="sxs-lookup"><span data-stu-id="6c49f-102">Intune Device Inventory</span></span>

<span data-ttu-id="6c49f-103">Oљtrica uređaja pruža administratorni uvid u "Uređaji" u okviru upravljanja u okviru usluge Intune na osnovu po uređaju.</span><span class="sxs-lookup"><span data-stu-id="6c49f-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="6c49f-104">Prikazane informacije uključuju: hardver, pronađene aplikacije, stanje usaglašenosti uređaja i stanje konfiguracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="6c49f-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="6c49f-105">Podaci o zalihama za hardver i otkrivene aplikacije se prikupljaju na sedmodnevnom ciklusu.</span><span class="sxs-lookup"><span data-stu-id="6c49f-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="6c49f-106">Prijave i određeni elementi hardvera prijavljeni su u zavisnosti od operativnog sistema uređaja i da li je uređaj lično ili u vlasništvu preduzeća.</span><span class="sxs-lookup"><span data-stu-id="6c49f-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="6c49f-107">Više informacija potražite u članku [Pregled detalja uređaja u programu Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="6c49f-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="6c49f-108">**NAJČEŠĆA PITANJA**</span><span class="sxs-lookup"><span data-stu-id="6c49f-108">**FAQ**</span></span>

<span data-ttu-id="6c49f-109">Q: ne primam kompletnu listu aplikacija koje su prisutne na Intune-upisanim Windows uređajima.</span><span class="sxs-lookup"><span data-stu-id="6c49f-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="6c49f-110">zašto da ne?</span><span class="sxs-lookup"><span data-stu-id="6c49f-110">Why not?</span></span>

<span data-ttu-id="6c49f-111">A: sada su navedene samo moderne aplikacije za Windows 10 računare koji su identifikovani kao korporativni uređaji.</span><span class="sxs-lookup"><span data-stu-id="6c49f-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="6c49f-112">Intune ne prikuplja informacije o Win32 aplikacijama instaliranih na ovim uređajima.</span><span class="sxs-lookup"><span data-stu-id="6c49f-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="6c49f-113">P: Zašto se brojevi telefona ne prikupljaju sa svih uređaja?</span><span class="sxs-lookup"><span data-stu-id="6c49f-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="6c49f-114">A: telefoni kategorizovani kao korporativni uređaji u Intune se ne identifikuju sa punim brojem telefona kada, na primer, pokrećete izveštaj o zalihama mobilnog uređaja.</span><span class="sxs-lookup"><span data-stu-id="6c49f-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="6c49f-115">Broj telefonskih brojeva sa doniranim uređajima je uvek delimično maskiran sa zvezdica (\* \* \* \*) i Prikaži samo poslednje četiri cifre.</span><span class="sxs-lookup"><span data-stu-id="6c49f-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>