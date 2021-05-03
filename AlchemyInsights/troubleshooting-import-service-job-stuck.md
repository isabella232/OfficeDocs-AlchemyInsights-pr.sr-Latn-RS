---
title: Rešavanje problema sa radom usluge uvoza je zaglavljen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125492"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="34705-102">Rešavanje problema sa radom usluge uvoza je zaglavljen</span><span class="sxs-lookup"><span data-stu-id="34705-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="34705-103">Ako nailazite na probleme sa poslovama uvoza usluga zaglavljenim ili neuspešnim, ispitajte i pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="34705-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="34705-104">Pregledajte veličinu PST datoteke.</span><span class="sxs-lookup"><span data-stu-id="34705-104">Review the size of of the PST file.</span></span> <span data-ttu-id="34705-105">Maksimalna preporučena veličina PST datoteke za uvoz je 20 GB.</span><span class="sxs-lookup"><span data-stu-id="34705-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="34705-106">Ako sumnjate da su preskočene stavke usled oštećenja, pokrenite Scanpst.exe da biste dijagnostikovali i otklonili greške u PST datotekama.</span><span class="sxs-lookup"><span data-stu-id="34705-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="34705-107">Ako vidite grešku "MapiExceptionShutoffQuotaExceed" tokom uvoza, uverite se da ciljno poštansko sanduče ima dovoljno kapaciteta za uvoz željenih PST datoteka.</span><span class="sxs-lookup"><span data-stu-id="34705-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="34705-108">Više informacija o rešavanju problema sa PST uvozom potražite u odeljku Rešavanje problema [sa alatkama za PST uvoz.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="34705-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="34705-109">Informacije o tome kako da rešite probleme prilikom uvoza PST datoteka u Outlook potražite u Outlook Rešavanje problema sa uvozom [Outlook .pst datoteke (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="34705-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>