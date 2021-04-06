---
title: Identifikovanje problema sa Windows virtuelnom radnom površinom
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595858"
---
# <a name="identify-windows-virtual-desktop-issues"></a>Identifikovanje problema sa Windows virtuelnom radnom površinom

Windows virtuelna dijagnostika radne površine koristi samo jednu PowerShell cmdlet komandu, ali sadrži mnogo opcionalnih parametara kako bi suzila i izolovao probleme. Da biste počeli: 

1. Preuzmite i uvezite modul Windows Virtual Desktop PowerShell. Više detalja možete da [vidite u temi Windows virtuelne radne površine za Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)

1. Pokrenite sledeću cmdlet cmdlet da biste se prijavili na svoj nalog:
    
    Primer: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**NAPOMOGUĆENO:** Svi upiti koji koriste PowerShell moraju da sadrže parametre -UserName ili -ActivityID. Mogućnosti nadgledanja možete da koristite za [funkciju dijagnostike](https://go.microsoft.com/fwlink/?linkid=2126847)pomoću funkcije evidencije.

Da biste filtrirali aktivnosti dijagnostike po korisniku, pokrenite sledeću cmdlet alatku:

Primer: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

Postoji lista filtera koje možete da pokrenete da biste dijagnostikovali probleme. Da biste saznali više o dijagnostikovanju problema, pogledajte tj. [identifikovanje i dijagnostikovanje problema sa Windows virtuelnom radnom površinom.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)

Da biste saznali više o uobičajenim greškama, pogledajte [uobičajene greške senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
