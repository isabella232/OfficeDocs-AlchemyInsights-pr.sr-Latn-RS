---
title: DLP pravilo za SSN ne radi
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679383"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="b55b5-102">DLP problemi sa brojevima socijalnog osiguranja</span><span class="sxs-lookup"><span data-stu-id="b55b5-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="b55b5-103">**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="b55b5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b55b5-104">**LINP problemi sa SNS-ovima**</span><span class="sxs-lookup"><span data-stu-id="b55b5-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="b55b5-105">Da li imate problema sa **prevencijom gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **broj socijalnog osiguranja (SSN)** kada koristite osetljiv tip informacija u usluzi Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="b55b5-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="b55b5-106">Ako je tako, uverite se da sadržaj sadrži potrebne informacije za ono što traži DLP smernice.</span><span class="sxs-lookup"><span data-stu-id="b55b5-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="b55b5-107">Na primer, za SSN smernice podešene pomoću nivoa pouzdanosti 85%, sledeće se procenjuju i mora se otkriti da bi pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="b55b5-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b55b5-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifara, što je možda u oblikovanom ili neoblikovanom obrascu</span><span class="sxs-lookup"><span data-stu-id="b55b5-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="b55b5-109">**[Obrazac:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSNs u četiri različita šablona:</span><span class="sxs-lookup"><span data-stu-id="b55b5-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="b55b5-110">Func_ssn pronalazi SSNs sa jakim oblikovanjem pre 2011 koje su oblikovane pomoću crtica ili razmaka (DDD-dd-dddd ili DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="b55b5-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="b55b5-111">Func_unformatted_ssn pronalazi Ssnsa sa jakim oblikovanjem pre 2011 koje su neoblikovane kao devet uzastopnih cifara (ddddddddddd)</span><span class="sxs-lookup"><span data-stu-id="b55b5-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="b55b5-112">Func_randomized_formatted_ssn pronalazi 2011 SSNs koji su oblikovani sa crtama ili razmacima (DDD-dd-dddd ili DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="b55b5-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="b55b5-113">Func_randomized_unformatted_ssn pronalazi 2011 SSNs koje nisu oblikovane kao devet uzastopnih cifara (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="b55b5-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="b55b5-114">Provera **[zbira:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, ne postoji kontrolni zbir</span><span class="sxs-lookup"><span data-stu-id="b55b5-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="b55b5-115">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Funkcija DLP je 85% uverena da otkriva ovaj tip osetljivih informacija ako u neposrednoj blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="b55b5-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b55b5-116">[Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) pronalazi sadržaj koji se podudara sa obrascem.</span><span class="sxs-lookup"><span data-stu-id="b55b5-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b55b5-117">Postoji ključna reč iz [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="b55b5-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="b55b5-118">Primeri ključnih reči uključuju:  *socijalnu bezbednost, socijalnu bezbednost #, soc sec, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="b55b5-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="b55b5-119">Na primer, sledeći uzorak će se pokrenuti za DP SSN smernice: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="b55b5-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="b55b5-120">Za više informacija o tome šta je potrebno da bi se Snsa otkrilo za vaš sadržaj, pogledajte sledeći odeljak u ovom članku: [Šta osetljive informacije tipovi traže za SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="b55b5-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="b55b5-121">Koristite drugačiji tip pristupačnije osetljive informacije, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="b55b5-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  