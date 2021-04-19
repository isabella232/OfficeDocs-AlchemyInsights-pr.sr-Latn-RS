---
title: Rešavanje problema PST uvoza
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
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826177"
---
# <a name="troubleshooting-pst-import-issues"></a>Rešavanje problema PST uvoza

- Ako uvozite unutar Outlook klijenta, pročitajte članak [Rešavanje problema prilikom uvoza Outlook. pst datoteke](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Ako koristite uslugu Uvoza i ona se zaglavi, imajte u vidu da svaka PST datoteka koju otpremate na lokaciju Azure skladišta ne bi trebalo da bude veća od 20 GB. PST datoteke veće od 20 GB mogu da utiču na performanse PST procesa uvoza.

- Ako želite da verifikujete status određenog zadatka uvoza, možete da koristite [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Za kompletne detalje o usluzi uvoza, pročitajte članak [Pregled uvoženja PST datoteka vaše organizacije](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
