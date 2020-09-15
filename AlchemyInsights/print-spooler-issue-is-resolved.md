---
title: Rešen je problem štampanja na čekanju
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801855"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="9a9ad-102">Rešen je problem štampanja na čekanju</span><span class="sxs-lookup"><span data-stu-id="9a9ad-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="9a9ad-103">Ako se uređaj ažurira pomoću operativnog sistema Windows 10  **OS Build 19041,329**, možda ste videli problem gde se određeni štampači ne štampaju.</span><span class="sxs-lookup"><span data-stu-id="9a9ad-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="9a9ad-104">Upravljač štampanja na čekanju može da napravi grešku ili se neočekivano zatvori prilikom pokušaja štampanja, a nijedan izlaz ne potiče od štampača koji je uticao na njega.</span><span class="sxs-lookup"><span data-stu-id="9a9ad-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="9a9ad-105">Ovaj problem je rešen u OS Build  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="9a9ad-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="9a9ad-106">**Trenutna istraga**</span><span class="sxs-lookup"><span data-stu-id="9a9ad-106">**Ongoing investigation**</span></span>

<span data-ttu-id="9a9ad-107">Datoteka datoteke lokalnog bezbednosnog autoriteta za uslugu lokalne bezbednosti (LSASS) (**Isass.exe**) može da ne uspe na nekoj uređaju sa porukom o grešci "kritični sistemski proces, C:\WINDOWS\system32\Isass.exe, nije uspeo sa statusnim kodom c0000008.</span><span class="sxs-lookup"><span data-stu-id="9a9ad-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="9a9ad-108">Mašina se sada mora ponovo pokrenuti ".</span><span class="sxs-lookup"><span data-stu-id="9a9ad-108">The machine must now be restarted".</span></span>  <span data-ttu-id="9a9ad-109">**Microsoft radi na rezoluciji i obezbediće ispravku u narednom izdanju.**</span><span class="sxs-lookup"><span data-stu-id="9a9ad-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="9a9ad-110">Više informacija potražite u  [verzijama poznatih problema sa operativnim sistemom Windows 10 Version 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="9a9ad-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>