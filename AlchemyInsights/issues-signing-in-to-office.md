---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579915"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prazan ekran za prijavljivanje u Microsoft 365 aplikacijama

Da biste rešili ovaj problem, pokušajte sledeće:
- Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Poništi opcije programa Internet Explorer: idi na **Alatke**  >  **Internet opcije**  >  **Napredno**  >  **uspostavljanje početnih vrednosti postavki programa Internet Explorer** (Imajte na umu da ćete izgubiti prilagođene postavke), a zatim ponovo pokušajte da se prijavite u Office.
- Onemogućite čuvar aplikacija Windows Defender (WDAG) ili neki sličan zaštitni zid ili program za zaštitu od virusa:
    1. Na kontrolnoj tabli idite na **programe**, a zatim odaberite **Uključivanje ili isključivanje funkcija operativnog sistema Windows**.
    2. Ako je čuvar aplikacije Windows Defender omogućen, pokušajte da ga onemogućite.<br/>
    **Napomena:** Možda ćete morati ponovo da pokrenete računar.
- Uverite se da se Microsoft. AAD. BrokerPlugin [AAD "Plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) " ne blokira ni jednom aplikacijom ili zaštitnim zidom/antivirusni program.
- [Obrišite Office akreditive](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) koristeći Windows upravljač akreditivima.<br/>
    **Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0. (Ex: \Software\microsoft\office\16.0\zajed\identitet\)

Više informacija potražite u članku [problemi prilikom prijavljivanja nakon ažuriranja na Office 2016 Build 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).