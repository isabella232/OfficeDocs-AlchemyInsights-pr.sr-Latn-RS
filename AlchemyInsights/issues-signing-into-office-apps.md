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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579879"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravka Microsoft 365 aplikacija "modul pouzdane platforme računara ne funkcioniše ispravno" poruka

Da biste ispravili ovu grešku, pokušajte sledeće:

- Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Obrišite Office akreditive](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) koristeći Windows upravljač akreditivima.<br/>
    **Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0. (Ex: \Software\microsoft\office\16.0\zajed\identitet\)
- Pokušajte sa [procesom oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste otklonili greške modula pouzdane platforme (TPM).
- Postavite Vodolovni potencijalnog klijenta = 0 koristeći sledeće korake:  
    1. Kliknite desnim tasterom miša na dugme "Start" operativnog sistema Windows, izaberite stavku **Pokreni**, otkucajte **Regedit**, a zatim odaberite **"u redu"**.
    2. Izaberite **da** da dozvolite Registry Editoru da napravi izmjene na vašem uređaju.
    3. U programu Registry Editor dodajte DWORD vrednost **Enabpotencijalnog klijenta** sa postavkom **0** ispod HKEY_CURRENT_USER \Software\microsoft\office\16.0\pod\identity.

Više informacija potražite u članku [problemi prilikom prijavljivanja nakon ažuriranja na Office 2016 Build 16.0.7967 na Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).