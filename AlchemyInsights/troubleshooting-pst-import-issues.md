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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972433"
---
# <a name="troubleshooting-pst-import-issues"></a>Rešavanje problema PST uvoza

- Ako uvozite u okviru samog Outlook, pogledajte rešavanje problema sa uvozom [Outlook .pst datoteke.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Ako koristite uslugu uvoza i ona je zaglavljena, imajte u nahu da svaka PST datoteka koju otpremite na Azure lokaciju skladišta ne bi trebalo da bude veća od 20 GB. PST datoteke veće od 20 GB mogu da utiču na performanse PST procesa uvoza. Više informacija o rešavanju problema sa zaglavljenim poslom potražite u [odeljku Problemi koji utiču na PST zadatak uvoza.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Ako želite da proverite status određenog posla uvoza, koristite [Get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Za sve detalje o usluzi uvoza pogledajte [Pregled uvoza PST datoteka organizacije.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
