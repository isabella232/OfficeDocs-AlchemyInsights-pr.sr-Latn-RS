---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
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
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833089"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Popravljanje Microsoft 365 aplikacije u kojoj je poruka "Žao nam je, drugi nalog vaše organizacije je već prijavljen"

Da biste ispravili ovu grešku, pokušajte sledeće:

- Uklonite sve radne naloge, osim naloga na koji ovo utiče pomoću postavki operativnog sistema Windows > **pristup poslu ili školi.**
- [Obriši Office akredile pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows upravljača akreditima.<br/>
    **Napomogućeno:** Putanje registratora za Office 2016 promenjene su u 16.0. (Na ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorite Office aplikaciju i odaberite stavku **Odjavi**  >  **se nalog**  >  **datoteke**. Zatim se prijavite pomoću korisničkog naloga sa važećom licencom. Detaljne informacije potražite u članku [Nalozi u sistemu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Za Mac računar pročitajte članak [Nije moguće prijaviti se u Office 2016 za Mac aplikaciju](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Dodatne informacije potražite u temi "Žao nam je, drugi nalog vaše organizacije je već [prijavljen na ovom računaru" u office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)