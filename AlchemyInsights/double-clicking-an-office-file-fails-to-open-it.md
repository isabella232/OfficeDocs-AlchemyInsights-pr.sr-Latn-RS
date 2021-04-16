---
title: Dvostrukim klikom na Office datoteku ne može se otvoriti datoteka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814819"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="7ab4b-102">Dvostrukim klikom na Office datoteku ne može se otvoriti datoteka</span><span class="sxs-lookup"><span data-stu-id="7ab4b-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="7ab4b-103">Kada kliknete dvaput na Office datoteku, možda ćete videti da je program otvoren, ali se sama datoteka ne otvara.</span><span class="sxs-lookup"><span data-stu-id="7ab4b-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="7ab4b-104">Ili ćete možda dobiti grešku: "Došlo je do problema prilikom slanja komande programu".</span><span class="sxs-lookup"><span data-stu-id="7ab4b-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="7ab4b-105">Postoji mnogo uzroka za ovo, ali dva najčešća rešenja su:</span><span class="sxs-lookup"><span data-stu-id="7ab4b-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="7ab4b-106">U programu Excel, uverite se da je opcionalna opcija DDE.</span><span class="sxs-lookup"><span data-stu-id="7ab4b-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="7ab4b-107">Opciju možete pronaći kreiranjem nove radne sveske, a zatim odabiti stavku Datoteka **> Opcije > Napredno**.</span><span class="sxs-lookup"><span data-stu-id="7ab4b-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="7ab4b-108">U **odeljku Opšte** poništite oznaku Zanemari druge aplikacije koje koriste **Dynamic Data Exchange (DDE).**</span><span class="sxs-lookup"><span data-stu-id="7ab4b-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="7ab4b-109">Pokrenite popravku na mreži da biste vratili podrazumevane postavke.</span><span class="sxs-lookup"><span data-stu-id="7ab4b-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="7ab4b-110">Kliknite na Dugme Windows Start i potražite stavku "Kontrolna tabla".</span><span class="sxs-lookup"><span data-stu-id="7ab4b-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="7ab4b-111">Otvorite **kontrolnu tablu** i idite na **stavku Programi > Programi i funkcije**.</span><span class="sxs-lookup"><span data-stu-id="7ab4b-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="7ab4b-112">Zatim kliknite desnim tasterom **miša na Microsoft Office [Verzija]** i odaberite stavku Promeni > **popravku na mreži.**</span><span class="sxs-lookup"><span data-stu-id="7ab4b-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="7ab4b-113">Ako nijedno od ovih rešenja ne funkcioniše, kompletniji spisak rešenja možete pronaći u članku podrške, dvostrukim klikom na Office datoteku ne možete da je [otvorite.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="7ab4b-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
