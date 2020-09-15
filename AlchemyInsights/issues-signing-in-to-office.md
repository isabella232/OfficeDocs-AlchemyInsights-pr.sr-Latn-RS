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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695301"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazan ekran za prijavljivanje u Microsoft 365 aplikacijama

Da biste rešili ovaj problem, pokušajte sledeće:
- Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Resetujte opcije programa Internet Explorer: idite na stavku **Alatke**  >  **Internet opcije**  >  **više**  >  puta**uspostavite početne vrednosti postavki programa Internet Explorer** (Imajte u vidu da ćete izgubiti prilagođene postavke), a zatim ponovo pokušajte da se prijavite u Office.
- Onemogućavanje čuvara aplikacije "Windows zaštitnik" (WDAG) ili sliиnog zaštitnog zida ili antivirusnog programa:
    1. Na kontrolnoj tabli idite na **Programi**, a zatim odaberite stavku **Uključi ili isključi Windows funkcije**.
    2. Ako je Windows Defender aplikacija omogućena, pokušajte da je onemogućite.<br/>
    **Napomena:** Možda ćete morati ponovo da pokrenete računar.
- Uverite se da dodatna komponenta Microsoft. AAD. Brokerstgin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne blokira bilo koju aplikaciju ili antivirusni program.
- [Brisanje Office akreditiva](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravljača Windows akreditivima.<br/>
    **Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0. (Ex: \Software\microsoft\office\16.0\local \ identitet\)

Više informacija potražite u članku [problemi sa vezom u prijavljivanju nakon ažuriranja na Office 2016 16.0.7967 u operativnom sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).