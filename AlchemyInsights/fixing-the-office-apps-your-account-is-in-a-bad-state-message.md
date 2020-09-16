---
title: Popravka Microsoft 365 aplikacija nalog se nalazi u lošoj državnoj poruci
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744559"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Popravka Microsoft 365 aplikacija "vaš nalog je u lošem stanju"

Da biste rešili ovu grešku, Isprobajte sledeće opcije na računaru koji je uticao:

- Otvorite Office aplikaciju, izaberite stavku **File**  >  **nalog**  >  **za datoteku iz svih naloga**. Ponovo se prijavite pomoću korisničkog naloga sa važećom licencom. Detaljne informacije potražite u članku [Nalozi u sistemu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Brisanje Office akreditiva](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravljača Windows akreditivima.<br>
  **Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0. Na primer, \Software\Microsoft\Office\16.0\Common\Identity\
- Ako se greška javlja prilikom povezivanja sa sistemom Office 365 pomoću sistema Office 2013, [omogućite modernu potvrdu identiteta](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) za Office klijent.

Više informacija potražite u članku [Rešavanje problema sa aplikacijama koje nisu pregledač koji ne mogu da se prijave u Microsoft 365, Azure ili Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

