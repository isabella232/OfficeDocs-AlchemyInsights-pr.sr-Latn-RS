---
title: SharePoint velika lista
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720147"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="0446c-102">Rad sa velikim listama i bibliotekama u sistemu SharePoint</span><span class="sxs-lookup"><span data-stu-id="0446c-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="0446c-103">SharePoint liste i biblioteke mogu da sadrže do 30.000.000 stavki, ali kada imaju više od 5.000 stavki, možda ćete videti grešku na pragu prikaza liste kada pokušate da radite sa njima.</span><span class="sxs-lookup"><span data-stu-id="0446c-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="0446c-104">Ova granična vrednost služi za održavanje performansi usluge.</span><span class="sxs-lookup"><span data-stu-id="0446c-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="0446c-105">Nije je moguće promeniti.</span><span class="sxs-lookup"><span data-stu-id="0446c-105">It can't be changed.</span></span> <span data-ttu-id="0446c-106">Da bi se izbegao ovaj prag:</span><span class="sxs-lookup"><span data-stu-id="0446c-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="0446c-107">**Koristite modernu**</span><span class="sxs-lookup"><span data-stu-id="0446c-107">**Use modern**</span></span>

<span data-ttu-id="0446c-108">Prikazi koji prikazuju mnoge stavke najbolje funkcionišu u modernom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="0446c-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="0446c-109">[Koristite moderno iskustvo](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) da biste izbegli greške koje ćete možda videti u klasičnom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="0446c-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="0446c-110">**Dodavanje indeksa**</span><span class="sxs-lookup"><span data-stu-id="0446c-110">**Add indexes**</span></span>

<span data-ttu-id="0446c-111">Kada filtrirate ili sortirate po koloni koja nema indeks, možda ćete videti poruku o grešci.</span><span class="sxs-lookup"><span data-stu-id="0446c-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="0446c-112">[Dodajte indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) ručno iz **postavki liste** u meniju postavke, a zatim **indeksirajte kolone**.</span><span class="sxs-lookup"><span data-stu-id="0446c-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="0446c-113">**Uređivanje prikaza liste**</span><span class="sxs-lookup"><span data-stu-id="0446c-113">**Edit the list view**</span></span>

<span data-ttu-id="0446c-114">Ako dođe do greške prilikom rada sa velikom listom, [uredite prikaz liste](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="0446c-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="0446c-115">Sledeće četiri promene će ukloniti greške na pragu prikaza liste.</span><span class="sxs-lookup"><span data-stu-id="0446c-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="0446c-116">Izvršite sva četiri promene da biste uklonili sve greške.</span><span class="sxs-lookup"><span data-stu-id="0446c-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="0446c-117">Ako i dalje dobijate greške, potvrdite izbor u polju za proveru [velike liste i biblioteke](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="0446c-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="0446c-118">Izaberite **nijednu** od **prve vrste po koloni** , a **zatim sortirate po koloni**.</span><span class="sxs-lookup"><span data-stu-id="0446c-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="0446c-119">Izaberite **nijednu** iz **prve grupe po koloni** , a **zatim u koloni**.</span><span class="sxs-lookup"><span data-stu-id="0446c-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="0446c-120">Izaberite stavku **nijedno** za sve kolone u odeljku **ukupne vrednosti** .</span><span class="sxs-lookup"><span data-stu-id="0446c-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="0446c-121">Opozovite izbor sve osim jedne kolone za prikaz iz odeljka " **kolone** ".</span><span class="sxs-lookup"><span data-stu-id="0446c-121">Deselect all but one column for display from the **Columns** section.</span></span>

