---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
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
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695337"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Popravka Microsoft 365 aplikacija "Žao nam je, drugi nalog iz vaše organizacije je već prijavljen"

Da biste ispravili ovu grešku, pokušajte sledeće:

- Uklanjanje svih naloga za posao, osim naloga koji je uticao, pomoću Windows postavki > **Access poslu ili školi**.
- [Brisanje Office akreditiva](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravljača Windows akreditivima.<br/>
    **Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0. (Ex: \Software\microsoft\office\16.0\local \ identitet\)
- Otvorite Office aplikaciju, odaberite stavku **File**  >  **nalog naloga**za datoteku  >  **Sign Out**. Zatim se prijavite pomoću korisničkog naloga sa važećom licencom. Detaljne informacije potražite u članku [Nalozi u sistemu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Za Mac računar pročitajte članak [Nije moguće prijaviti se u Office 2016 za Mac aplikaciju](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Više informacija potražite u članku ["Žao nam je, drugi nalog iz vaše organizacije je već prijavljen na ovom računaru" u sistemu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).