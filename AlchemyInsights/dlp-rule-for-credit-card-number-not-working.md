---
title: DLP pravilo za broj kreditne kartice ne radi
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679455"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="a1575-102">DLP problemi sa brojevima kreditnih kartica</span><span class="sxs-lookup"><span data-stu-id="a1575-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="a1575-103">**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a1575-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a1575-104">**DLP problemi sa brojevima kreditnih kartica**</span><span class="sxs-lookup"><span data-stu-id="a1575-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="a1575-105">Da li imate problema sa **prevencijom gubitka podataka (dlp)** ne radi za sadržaj koji sadrži **broj kreditne kartice** prilikom korišćenja tipa dlp osetljive informacije u programu O365?</span><span class="sxs-lookup"><span data-stu-id="a1575-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="a1575-106">Ako je tako, uverite se da sadržaj sadrži potrebne informacije za pokretanje DLP smernica kada se proceni.</span><span class="sxs-lookup"><span data-stu-id="a1575-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="a1575-107">Na primer, za **smernice kreditne kartice** podešene pomoću nivoa pouzdanosti 85%, sledeće se procenjuju i mora se otkriti da bi pravilo pokrenulo:</span><span class="sxs-lookup"><span data-stu-id="a1575-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="a1575-108">**[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifara koje mogu da se oblikuju ili neoblikovane (dddddddddddddddd) i moraju da proslede luhn test.</span><span class="sxs-lookup"><span data-stu-id="a1575-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="a1575-109">**[Obrazac:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Veoma složen i robusan šara koji prepoznaje kartice svih velikih brendova širom sveta, uključujući vizu, MasterCard, karticu otkrivanja, JCB, American Express, poklon-razglednice i иestitke za restoran.</span><span class="sxs-lookup"><span data-stu-id="a1575-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="a1575-110">Provera **[zbira:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, polje "Luhn"</span><span class="sxs-lookup"><span data-stu-id="a1575-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="a1575-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Funkcija DLP je 85% uverena da otkriva ovaj tip osetljivih informacija ako u neposrednoj blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="a1575-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="a1575-112">Funkcija Func_credit_card pronalazi sadržaj koji se podudara sa obrascem.</span><span class="sxs-lookup"><span data-stu-id="a1575-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="a1575-113">Tačno:</span><span class="sxs-lookup"><span data-stu-id="a1575-113">One of the following is true:</span></span>

  - <span data-ttu-id="a1575-114">Postoji ključna reč iz Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="a1575-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="a1575-115">Pronađena je ključna reč iz Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="a1575-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="a1575-116">Funkcija Func_expiration_date pronalazi datum u pravom formatu za datum.</span><span class="sxs-lookup"><span data-stu-id="a1575-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="a1575-117">Propusnice za proveru</span><span class="sxs-lookup"><span data-stu-id="a1575-117">The checksum passes</span></span>

    <span data-ttu-id="a1575-118">Na primer, sledeći uzorak će se pokrenuti radi smernica za DEP kreditnu karticu:</span><span class="sxs-lookup"><span data-stu-id="a1575-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="a1575-119">Viza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="a1575-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="a1575-120">Ističe: 2/2009</span><span class="sxs-lookup"><span data-stu-id="a1575-120">Expires: 2/2009</span></span>

<span data-ttu-id="a1575-121">Više informacija o tome šta je potrebno da bi se video **broj kreditne kartice** detektovano za sadržaj potražite u sledećem odeljku u ovom članku: [koje vrste osetljivim informacija traže kreditnu karticu "](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="a1575-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="a1575-122">Koristite drugačiji tip pristupačnije osetljive informacije, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="a1575-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  