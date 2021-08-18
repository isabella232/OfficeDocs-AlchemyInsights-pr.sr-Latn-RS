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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088050"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazan ekran za prijavljivanje u Microsoft 365 aplikacijama

Da biste rešili ovaj problem, pokušajte sledeće:
- Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Kancelarija.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Uspostavite početne vrednosti opcija programa Internet Explorer: Idite na Alatke Internet opcije Napredne opcije za poništavanje programa Internet Explorer Postavke (imajte u Postavke da ćete izgubiti prilagođene postavke), a zatim pokušajte ponovo da se  >    >    >   prijavite u Kancelarija programa.
- Onemogućite Application Guard Windows zaštitnika (WDAG) ili bilo koji sličan zaštitni zid ili antivirusni program:
    1. Na kontrolnoj tabli izaberite **stavku Programi**, a zatim odaberite Windows uključivanje ili **isključivanje funkcija programa**.
    2. Ako Application Guard Windows zaštitnika funkciju omogućena, pokušajte da je onemogućite.<br/>
    **Napomogućeno:** Možda ćete morati ponovo da pokrenete računar.
- Uverite se da aplikacija ili programski dodatak Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne blokira nijednu aplikaciju ili zaštitni zid/antivirusni program.
- [Opozovite Kancelarija akreditiva pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows akreditiva.<br/>
    **Napomogućeno:** Putanje registratora za Kancelarija 2016 su promenjene na 16.0. (Na ex: \Software\Microsoft\Kancelarija\16.0\Common\Identity\)

Više informacija potražite u temi Problemi sa povezivanjem pri prijavljivanjem nakon ažuriranja za [Kancelarija 2016 izdanje 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)na Windows 10.