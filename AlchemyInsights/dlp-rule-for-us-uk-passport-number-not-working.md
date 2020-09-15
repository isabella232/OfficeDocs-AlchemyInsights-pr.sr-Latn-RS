---
title: DLP pravilo za broj pasoša nam/UK ne radi
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679238"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="0e381-102">Problemi sa brojevima DLP-američko/UK pasoša</span><span class="sxs-lookup"><span data-stu-id="0e381-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="0e381-103">**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="0e381-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0e381-104">**DP problemi sa brojevima pasoša američkih/BRITANIJA**</span><span class="sxs-lookup"><span data-stu-id="0e381-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="0e381-105">Da li imate problema sa **prevencijom gubitka podataka (dlp)** ne radi za sadržaj koji sadrži **broj američkog/britanskog pasoša** kada koristite Tip informacija osetljive na dlp u O365?</span><span class="sxs-lookup"><span data-stu-id="0e381-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0e381-106">Ako je tako, uverite se da sadržaj sadrži potrebne informacije za šta su smernice za DLP traženi prilikom procene.</span><span class="sxs-lookup"><span data-stu-id="0e381-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="0e381-107">Na primer, za smernice sa **američkom/britanski pasošem brojevima** podešene pomoću nivoa pouzdanosti 75%, sledeće se procenjuju i mora se otkriti da bi pravilo pokrenulo</span><span class="sxs-lookup"><span data-stu-id="0e381-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="0e381-108">**[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet cifara</span><span class="sxs-lookup"><span data-stu-id="0e381-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="0e381-109">**[Obrazac:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet uzastopnih cifara</span><span class="sxs-lookup"><span data-stu-id="0e381-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="0e381-110">Provera **[zbira:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji kontrolni zbir</span><span class="sxs-lookup"><span data-stu-id="0e381-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="0e381-111">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Funkcija DLP je 75% uverena da otkriva ovaj tip osetljivih informacija ako u neposrednoj blizini 300 znakova:</span><span class="sxs-lookup"><span data-stu-id="0e381-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0e381-112">Funkcija Func_usa_uk_passport pronalazi sadržaj koji se podudara sa obrascem.</span><span class="sxs-lookup"><span data-stu-id="0e381-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0e381-113">Postoji ključna reč iz Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="0e381-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="0e381-114">Na primer, sledeći uzorak će se pokrenuti za polisu za **američke/britanski pasoš broj** : američki pasoš broj 123456789</span><span class="sxs-lookup"><span data-stu-id="0e381-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="0e381-115">Više informacija o tome šta je potrebno za broj za AMERIČKI/britanski pasoš da bi se otkrilo za vaš sadržaj potražite u sledećem odeljku u ovom članku: [Šta osetljive informacije tipovi traže za američki/britanski pasoš broj pasoša](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="0e381-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="0e381-116">Koristite drugačiji tip pristupačnije osetljive informacije, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="0e381-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  