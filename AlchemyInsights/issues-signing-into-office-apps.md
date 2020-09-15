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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695193"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Popravka Microsoft 365 aplikacija "modul pouzdane platforme računara ne radi ispravno" poruka

Da biste ispravili ovu grešku, pokušajte sledeće:

- Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Brisanje Office akreditiva](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravljača Windows akreditivima.<br/>
    **Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0. (Ex: \Software\microsoft\office\16.0\local \ identitet\)
- Isprobajte [proces oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) za popravljanje otkazivanja modula pouzdane platforme (TPM).
- Postavljanje programskog programskog + = 0 pomoću sledećih koraka:  
    1. Kliknite desnim tasterom miša na dugme Start operativnog sistema Windows, odaberite stavku **Pokreni**, otkucajte **ponovno gedit**, a zatim odaberite stavku **u redu**.
    2. Kliknite na dugme **da** da biste omogućili uređivaču registratora da napravi promene na uređaju.
    3. U uređivaču registratora dodajte DWORD vrednost programskog **dodatka sa** podešavanjem **0** u okviru HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Više informacija potražite u članku [problemi sa vezom u prijavljivanju nakon ažuriranja na Office 2016 16.0.7967 u operativnom sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).