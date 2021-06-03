---
title: DLP krajnja tačka nije primenjena na uređaj korisnika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731866"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP krajnja tačka nije primenjena na uređaj korisnika

Ako postavka sprečavanja gubitka podataka krajnje tačke (DLP) nije primenjena na uređaj korisnika, proverite da li ispunjavate ove zahteve:

- Windows 10 x64 operativnog sistema 1809 ili novija, instalirana je na uređaju.
- Instalirana je verzija klijenta za borbu protiv malvera 4.18.2009.7 ili novija.
- Uređaj je **jedan od** ovih:
    
    - Azure Active Directory (Azure AD) pridružen
    - Hibridni Azure AD pridružen
    - AAD registrovan

- Da biste na primenili radnje smernica, proverite Chromium pregledač Microsoft Chromium Edge instaliran na uređaju krajnje tačke.

Dodatne zahteve za primenu DLP krajnje tačke možete da dobijete u temi Prvi koraci uz sprečavanje [gubitka podataka krajnje tačke.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)