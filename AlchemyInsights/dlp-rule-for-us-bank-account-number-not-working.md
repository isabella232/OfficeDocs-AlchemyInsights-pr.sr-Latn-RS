---
title: DLP pravilo za broj računa u banci za sad ne radi
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679310"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="a5de4-102">DLP problemi sa brojevima američkih računa u banci</span><span class="sxs-lookup"><span data-stu-id="a5de4-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="a5de4-103">**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a5de4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a5de4-104">**DLP problemi sa brojevima američkih računa u banci**</span><span class="sxs-lookup"><span data-stu-id="a5de4-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="a5de4-105">Da li imate problema sa **prevencijom gubitka podataka (dlp)** ne radi za sadržaj koji sadrži **broj računa američkog banke** prilikom korišćenja dlp osetljive informacije u programu O365?</span><span class="sxs-lookup"><span data-stu-id="a5de4-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a5de4-106">Ako je tako, uverite se da sadržaj sadrži potrebne informacije za šta su smernice za DLP traženi prilikom procene.</span><span class="sxs-lookup"><span data-stu-id="a5de4-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="a5de4-107">Na primer, za polise **broja američkih računa u banci** podešene pomoću nivoa pouzdanosti 85%, sledeće se procenjuju i mora se otkriti da bi pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="a5de4-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a5de4-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifara</span><span class="sxs-lookup"><span data-stu-id="a5de4-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="a5de4-109">**[Šara:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 uzastopnih cifara.</span><span class="sxs-lookup"><span data-stu-id="a5de4-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="a5de4-110">Provera **[zbira:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji kontrolni zbir</span><span class="sxs-lookup"><span data-stu-id="a5de4-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="a5de4-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Funkcija DLP je 75% uverena da otkriva ovaj tip osetljivih informacija ako u neposrednoj blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="a5de4-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a5de4-112">Redovni izraz Regex_usa_bank_account_number pronalazi sadržaj koji se podudara sa šarom</span><span class="sxs-lookup"><span data-stu-id="a5de4-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="a5de4-113">Postoji ključna reč iz Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="a5de4-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="a5de4-114">Na primer, sledeći uzorak će se pokrenuti za polise **broja američkih bankovnih računa** : proveravanje naloga 78344011</span><span class="sxs-lookup"><span data-stu-id="a5de4-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="a5de4-115">Za više informacija o tome šta je potrebno da bi se otkrio **broj broja američkog bankovnog računa** za sadržaj, pogledajte sledeći odeljak u ovom članku: [Šta osetljive informacije tipovi traže za broj američkog bankovnog računa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="a5de4-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="a5de4-116">Koristite drugačiji tip pristupačnije osetljive informacije, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="a5de4-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  