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
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028054"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Popravljanje Microsoft 365 aplikacije "Žao nam je, drugi nalog vaše organizacije je već prijavljen"

Da biste ispravili ovu grešku, pokušajte sledeće:

- Uklonite sve radne naloge, osim ugroženog naloga, koristeći Windows Postavke > **pristup poslu ili školi.**
- [Opozovite Kancelarija akreditiva pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows akreditiva.<br/>
    **Napomogućeno:** Putanje registratora za Kancelarija 2016 su promenjene na 16.0. (Na ex: \Software\Microsoft\Kancelarija\16.0\Common\Identity\)
- Otvorite nalog aplikacija Office odaberite stavku **Odjavi se**  >  **nalog**  >  **datoteke.** Zatim se prijavite pomoću korisničkog naloga sa važećom licencom. Detaljne informacije potražite u članku [Nalozi u sistemu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Za Mac računar pročitajte članak [Nije moguće prijaviti se u Office 2016 za Mac aplikaciju](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Dodatne informacije potražite u [temi "Žao nam je,](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)drugi nalog vaše organizacije je već prijavljen na ovom računaru" na Kancelarija.