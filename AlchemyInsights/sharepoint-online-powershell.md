---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830596"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Radite sa programom PowerShell ili skriptima u okviru usluge SharePoint Online? Posetite veze u nastavku da biste dobili više informacija.
- [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Povezivanje sa uslugom SPO PowerShell pomoću višestruke potvrde identiteta (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- SharePoint obrasci i prakse [(PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sadrži biblioteku PowerShell komandi koja vam omogućava da izvršite složene radnje upravljanja prema SPO- u.

> [!NOTE]
> - Ako imate problema sa povezivanjem sa sistemom SPO management shell, [uverite](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) se da ste ažurirali na najnoviju verziju i pokušajte ponovo da uvezete modul pomoću *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Ako pokušavate da pokrenete skripte modela objekta na strani klijenta, morate da imate [SDK](https://www.microsoft.com/download/details.aspx?id=42038) za Sharepoint Online klijentske komponente instaliran na lokalnom računaru.
> - Ako imate problema sa pokretanjem skripti iz usluge PowerShell, možda ćete želeti da razmotrite pokretanje usluge PowerShell kao administratora i promenu smernica [za izvršavanje.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)