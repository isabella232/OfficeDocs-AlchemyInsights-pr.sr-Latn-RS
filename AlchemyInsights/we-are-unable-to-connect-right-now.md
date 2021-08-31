---
title: Problem sa aktivaciju – Trenutno ne možemo da se povežemo
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
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744609"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje Microsoft 365 "Trenutno ne možemo da se povežemo"

Na primer: Ako koristite stariju verziju programa Windows (na primer Windows 7 SP1, Windows Server 2008 R2), koristite jednostavnu popravku da biste kao podrazumevano omogućili TLS 1.2. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Više informacija potražite u temi Ažuriranje da biste omogućili [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao podrazumevane bezbedne protokole u winHTTP-u Windows.

Ako primite ovu poruku, pokušajte sledeće:

1. Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama. Pogledajte [članak Microsoft opsezi UL adresa i IP adresa.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Idite na **Start**  >  **Run**, a zatim **otkucajte services.msc**. Uverite se da su sve sledeće usluge pokrenute:
    - Automatsko podešavanje uređaja koji su povezani sa mrežom
    - Usluga "Lista mreža"
    - Svest o mrežnoj lokaciji
    - Windows Evidencija događaja

Ako jedna od ovih usluga nije pokrenuta, pokušajte da je pokrenete. Ako imate problema sa pokretanjem usluge, pokrenite sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:

**sfc /scannow**

Kada se ova komanda završi, ponovo pokrenite računar.

Detaljne informacije potražite u [temi "Žao nam je, ne možemo da se povežemo sa vašim nalogom. Greška "Pokušajte ponovo kasnije" kada aktivirate ovu Kancelarija sa Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)