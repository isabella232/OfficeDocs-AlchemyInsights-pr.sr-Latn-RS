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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709120"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravka Microsoft 365 aplikacija "modul pouzdane platforme računara ne radi ispravno" poruka

Da biste ispravili ovu grešku, pokušajte sledeće:

- Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Brisanje Office akreditiva](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) pomoću upravljača Windows akreditivima.<br/>
    **Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0. (Ex: \Software\microsoft\office\16.0\local \ identitet\)
- Isprobajte [proces oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) za popravljanje otkazivanja modula pouzdane platforme (TPM).
- Postavljanje programskog programskog + = 0 pomoću sledećih koraka:  
    1. Kliknite desnim tasterom miša na dugme Start operativnog sistema Windows, odaberite stavku **Pokreni**, otkucajte **ponovno gedit**, a zatim odaberite stavku **u redu**.
    2. Kliknite na dugme **da** da biste omogućili uređivaču registratora da napravi promene na uređaju.
    3. U uređivaču registratora dodajte DWORD vrednost programskog **dodatka sa** podešavanjem **0** u okviru HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Više informacija potražite u članku [problemi sa vezom u prijavljivanju nakon ažuriranja na Office 2016 16.0.7967 u operativnom sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).