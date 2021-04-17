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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833018"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Rešavanje poruke o Microsoft 365 aplikacijama "Modul pouzdane platforme na računaru ne funkcioniše ispravno"

Da biste ispravili ovu grešku, pokušajte sledeće:

- Instalirajte najnovije ispravke za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) i [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Obriši Office akredile pomoću](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows upravljača akreditima.<br/>
    **Napomogućeno:** Putanje registratora za Office 2016 promenjene su u 16.0. (Na ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Isprobajte proces [oporavka korisnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) da biste rešili probleme sa modulom pouzdane platforme (TPM).
- Podesite EnableADAL = 0 na sledeći način:  
    1. Kliknite desnim tasterom miša na Windows Start dugme, odaberite **stavku Pokreni**, **otkucajte regedit**, a zatim kliknite na dugme **U redu.**
    2. Kliknite na **dugme Da** da biste dozvolili uređivaču registratora da unosi promene na uređaju.
    3. U uređivaču registratora dodajte DWORD vrednost **funkcije EnableADAL** sa postavkom 0 u **okviru** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Više informacija potražite u temi Problemi sa povezivanjem pri prijavljivanjem nakon ažuriranja sistema [Office 2016 izdanje 16.0.7967](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)u operativnom sistemu Windows 10.