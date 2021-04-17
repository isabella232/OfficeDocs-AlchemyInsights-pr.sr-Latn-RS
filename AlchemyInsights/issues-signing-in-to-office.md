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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833053"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazan ekran za prijavljivanje u Microsoft 365 aplikacijama

Da biste rešili ovaj problem, pokušajte sledeće:
- Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Uspostavite početne vrednosti opcija u programu Internet Explorer: Idite na Alatke Internet opcije Napredne postavke programa  >    >    >  **Internet Explorer** (imajte naznaku da ćete izgubiti prilagođene postavke), a zatim pokušajte ponovo da se prijavite u Office.
- Onemogućite Application Guard Windows zaštitnik (WDAG) ili bilo koji sličan zaštitni zid ili antivirusni program:
    1. Na kontrolnoj tabli idite na **stavku Programi**, a zatim odaberite stavku Uključivanje ili **isključivanje Funkcija operativnog sistema Windows.**
    2. Ako je Application Guard Windows zaštitnik omogućen, pokušajte da ga onemogućite.<br/>
    **Napomogućeno:** Možda ćete morati ponovo da pokrenete računar.
- Uverite se da aplikacija ili programski dodatak Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ne blokira nijednu aplikaciju ili zaštitni zid/antivirusni program.
- [Obriši Office akredile pomoću](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows upravljača akreditima.<br/>
    **Napomogućeno:** Putanje registratora za Office 2016 promenjene su u 16.0. (Na ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Više informacija potražite u temi Problemi sa povezivanjem pri prijavljivanjem nakon ažuriranja sistema [Office 2016 izdanje 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)u operativnom sistemu Windows 10.