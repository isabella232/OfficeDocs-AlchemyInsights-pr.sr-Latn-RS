---
title: Funkcija DLP možda treba da bude prilagođen
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712198"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="e4e43-102">Funkcija DLP možda treba da bude prilagođen</span><span class="sxs-lookup"><span data-stu-id="e4e43-102">DLP might need a custom type</span></span>

<span data-ttu-id="e4e43-103">**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="e4e43-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="e4e43-104">**Funkcija DLP može zahtevati prilagođeni tip informacija**</span><span class="sxs-lookup"><span data-stu-id="e4e43-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="e4e43-105">Pomoću smernica za sprečavanje gubitka podataka (DLP) možete da identifikujete i zaštitite osetljive podatke u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="e4e43-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="e4e43-106">U nekoliko slučajeva možda ćete morati da kreirate sopstveni **prilagođeni** tip informacija da biste zaštitili podatke organizacije.</span><span class="sxs-lookup"><span data-stu-id="e4e43-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="e4e43-107">Na primer, vaša organizacija će možda morati da identifikuje i zaštiti ID-ove zaposlenih ili druge podatke u nekom formatu koji je specifičan za org. Ako je tako, pogledajte sledeće članke za više informacija.</span><span class="sxs-lookup"><span data-stu-id="e4e43-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="e4e43-108">**Prilagođavanje ugrađenog tipa informacija**</span><span class="sxs-lookup"><span data-stu-id="e4e43-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="e4e43-109">Ako tip ugrađene osetljive informacije odgovara vašim potrebama samo sa nekoliko dodataka, možete da [prilagodite ugrađeni tip informacija](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="e4e43-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="e4e43-110">Na primer, možete da dodate ili uklonite ključne reči ili da dodate ili uklonite pomoćne dokaze kao što je datum ili adresa.</span><span class="sxs-lookup"><span data-stu-id="e4e43-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="e4e43-111">**Kreiranje tipa prilagođene osetljive informacije**</span><span class="sxs-lookup"><span data-stu-id="e4e43-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="e4e43-112">Međutim, ako treba da identifikujete i zaštitite drugačiji tip osetljivih informacija, možete da [kreirate prilagođeni tip informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) u usluzi UI centra za usaglašenost &.</span><span class="sxs-lookup"><span data-stu-id="e4e43-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="e4e43-113">**Kreiranje prilagođene osetljive informacije u programu Security & centar za usaglašenost sa PowerShell**</span><span class="sxs-lookup"><span data-stu-id="e4e43-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="e4e43-114">Na kraju, ako UI ne obezbede sve opcije koje su vam potrebne, možete da [kreirate prilagođeni tip informacija u bezbednosnoj & PowerShell Center usaglašenosti](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="e4e43-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="e4e43-115">Ako počnete sa XML datotekom, možete da koristite svaku dostupnu opciju.</span><span class="sxs-lookup"><span data-stu-id="e4e43-115">By starting with an XML file, you can use every option available.</span></span>
