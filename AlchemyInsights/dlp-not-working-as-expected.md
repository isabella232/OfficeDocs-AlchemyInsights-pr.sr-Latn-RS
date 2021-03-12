---
title: DLP ne radi na očekivani način
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707824"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="0eda3-102">DLP ne radi na očekivani način</span><span class="sxs-lookup"><span data-stu-id="0eda3-102">DLP not working as expected</span></span>

<span data-ttu-id="0eda3-103">**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="0eda3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="0eda3-104">**Podešavanje DLP**</span><span class="sxs-lookup"><span data-stu-id="0eda3-104">**Setting up DLP**</span></span>

<span data-ttu-id="0eda3-105">Da li imate problema sa **prevencijom gubitka podataka (DLP)** u sistemu Office 365 ne radite kao što je očekivano?</span><span class="sxs-lookup"><span data-stu-id="0eda3-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="0eda3-106">Ako je tako, proverite da li su **smernice za dlp** ispravno podešene i da vaši podaci sadrže ono što traži **dlp smernice** kada se procenjuje.</span><span class="sxs-lookup"><span data-stu-id="0eda3-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="0eda3-107">DLP smernice vam omogućavaju da identifikujete i zaštitite osetljive informacije u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="0eda3-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="0eda3-108">Da biste postavili programe DLP, koristite ove informacije [ovde](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span><span class="sxs-lookup"><span data-stu-id="0eda3-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="0eda3-109">**Koje programe za DLP traže**</span><span class="sxs-lookup"><span data-stu-id="0eda3-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="0eda3-110">Kada koristite **ugrađene osetljive tipove informacija** u centrima bezbednosti i usaglašenosti, dlp smernice traže specifične obrasce i elemente prilikom detekcija ovih osetljivih tipova.</span><span class="sxs-lookup"><span data-stu-id="0eda3-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="0eda3-111">**Ugrađeni osetljivi tipovi informacija**</span><span class="sxs-lookup"><span data-stu-id="0eda3-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="0eda3-112">Informacije o ugrađenim osetljivim tipovima i tome koje smernice za DLP traže kada otkrivaju osetljiv tip, pogledajte članak: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="0eda3-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="0eda3-113">**Tipovi prilagođenih informacija**</span><span class="sxs-lookup"><span data-stu-id="0eda3-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="0eda3-114">Ako pokušavate da kreirate prilagođene osetljive informacije, koristite sledeći članak za informacije o tome kako da kreirate prilagođeni osetljivi tip [informacija: Kreirajte tip prilagođene osetljive informacije](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="0eda3-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="0eda3-115">**Testiranje DP smernica**</span><span class="sxs-lookup"><span data-stu-id="0eda3-115">**Test a DLP policy**</span></span>

<span data-ttu-id="0eda3-116">Da biste testirali podatke sa ugrađenim ili prilagođene osetljive informacije, koristite opciju **tip testa** u okviru **klasifikacija**  >  **osetljivih informacija**.</span><span class="sxs-lookup"><span data-stu-id="0eda3-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="0eda3-117">Više informacija potražite u članku [testiranje tipova prilagođenih osetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="0eda3-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="0eda3-118">**O**</span><span class="sxs-lookup"><span data-stu-id="0eda3-118">**Reports**</span></span>
  
- <span data-ttu-id="0eda3-119">Nabavite osetljive informacije [o Dlp izveštajima.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="0eda3-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="0eda3-120">Pogledajte određene detalje događaja sa [izveštajem o incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="0eda3-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
