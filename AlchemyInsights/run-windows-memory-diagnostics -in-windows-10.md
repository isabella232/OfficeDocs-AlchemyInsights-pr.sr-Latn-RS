---
title: Pokretanje Windows dijagnostike memorije u operativnom sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826681"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="e2095-102">Pokretanje Windows dijagnostike memorije u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="e2095-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="e2095-103">Ako Windows i aplikacije na računaru padnu, zamrznu se ili se ponašaju nestabilno, možda ćete naići na problem sa memorijom računara (RAM).</span><span class="sxs-lookup"><span data-stu-id="e2095-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="e2095-104">Možete da pokrenete Windows dijagnostiku memorije da biste proverili da li ima problema sa RAM memorijom računara.</span><span class="sxs-lookup"><span data-stu-id="e2095-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="e2095-105">U polje za pretragu na traci zadataka ukucajte **dijagnostika memorije**, a zatim izaberite **stavku Windows dijagnostika memorije**.</span><span class="sxs-lookup"><span data-stu-id="e2095-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="e2095-106">Da biste pokrenuli dijagnostiku, računar mora ponovo da se pokrene.</span><span class="sxs-lookup"><span data-stu-id="e2095-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="e2095-107">Imate opciju da odmah ponovo pokrenete (sačuvajte to što ste naveli i prvo zatvorite otvorene dokumente i e-poruke) ili da zakažete da se dijagnostika pokreće automatski kada se računar sledeći put pokrene:</span><span class="sxs-lookup"><span data-stu-id="e2095-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows dijagnostika memorije](media/windows-memory-diagnostic.png)

<span data-ttu-id="e2095-109">Kada se računar ponovo pokrene, Windows alatka za **dijagnostiku memorije** će se automatski pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="e2095-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="e2095-110">Status i napredak prikazuju se dok se dijagnostika pokreće, a vi možete da otkažete dijagnostiku tako što ćete pritisnuti taster **ESC** na tastaturi.</span><span class="sxs-lookup"><span data-stu-id="e2095-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="e2095-111">Kada se dijagnostika završi, Windows će početi normalno.</span><span class="sxs-lookup"><span data-stu-id="e2095-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="e2095-112">Odmah nakon ponovnog pokretanja, kada se radna  površina pojavi, pojaviće se obaveštenje (pored ikone centra za obaveštenja na traci zadataka) koje ukazuje na to da li su pronađene bilo kakve greške u memoriji.</span><span class="sxs-lookup"><span data-stu-id="e2095-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="e2095-113">Na primer:</span><span class="sxs-lookup"><span data-stu-id="e2095-113">For example:</span></span>

<span data-ttu-id="e2095-114">Evo ikone centra aktivnosti:</span><span class="sxs-lookup"><span data-stu-id="e2095-114">Here's the Action Center icon:</span></span> ![Ikona centra aktivnosti](media/action-center-icon.png) 

<span data-ttu-id="e2095-116">I probno obaveštenje:</span><span class="sxs-lookup"><span data-stu-id="e2095-116">And a sample notification:</span></span> ![Nema grešaka u memoriji](media/no-memory-errors.png)

<span data-ttu-id="e2095-118">Ako ste propustili obaveštenje, možete da izaberete ikonu  centra za obaveštenja na traci zadataka da biste prikazali centar za obaveštenja i videli listu obaveštenja koja se može pomerati. </span><span class="sxs-lookup"><span data-stu-id="e2095-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="e2095-119">Da biste pregledali detaljne informacije, **otkucajte događaj u** polje za pretragu na traci zadataka, a zatim izaberite **stavku Prikazivač događaja**.</span><span class="sxs-lookup"><span data-stu-id="e2095-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="e2095-120">U **oknu "Prikazivač** događaja" sa leve strane, izaberite stavke **Windows evidencije > Sistem**.</span><span class="sxs-lookup"><span data-stu-id="e2095-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="e2095-121">U desnom oknu pregledajte listu dok  gledate kolonu Izvor dok ne vidite događaje sa izvornom vrednošću **MemoryDiagnostics-Results.**</span><span class="sxs-lookup"><span data-stu-id="e2095-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="e2095-122">Istaknite svaki takav događaj i pogledajte informacije o rezultatima u okviru ispod **kartice** Opšte ispod liste.</span><span class="sxs-lookup"><span data-stu-id="e2095-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
