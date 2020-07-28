---
title: Kontrolisanje automatskih ispravki za Office aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439923"
---
# <a name="control-automatic-updates-for-office-apps"></a>Kontrolisanje automatskih ispravki za Office aplikacije

Podrazumevano, ispravke za Office aplikacije se preuzimaju automatski i primenjuju u pozadini bez intervencije korisnika. Međutim, administratori mogu da kontrolišu način na koji se ispravke primenjuju pomoću postavki Office Update. Postavke ažuriranja omogućavaju administratorima da omoguće ili onemoguće automatsko ažuriranje, da prikažu ili sakriju dugme " **Ažuriraj odmah** " u sistemu Office, postave rokove ažuriranja i još mnogo toga. Detaljnije informacije potražite u članku:

- [Konfigurišite postavke ažuriranja za Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatsko ažuriranje za Office nije omogućeno](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definišite kako će se Office ažurirati nakon instalacije](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Da biste redigovali postojeće postavke za ažuriranje primenjene na klijentsku mašinu, slijedite ove korake:

1. Otvorite alatku "Uređivač registratora" tako što ćete **pokrenuti**  >  **Run**  >  **program Regedit**.
2. Prebacite se na sledeću lokaciju i Pregledajte postavke za Office Update:  
    A. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    B. Konplje\konfiguracija

**Belešku**  Ako je ključ OfficeMgmtCOM postavljen, možda ćete videti poruku "ispravke kojima upravlja administrator sistema" na **Office**  >  **nalozima Office naloga**  >  **Office Updates**. Više informacija potražite u članku [Upravljanje ispravkama za microsoft 365 aplikacije pomoću upravljača za konfiguraciju krajnje tačke sistema Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  