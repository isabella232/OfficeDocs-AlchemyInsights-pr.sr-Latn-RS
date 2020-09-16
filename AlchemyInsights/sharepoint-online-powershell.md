---
title: SharePoint online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770853"
---
# <a name="sharepoint-online-powershell"></a>SharePoint online PowerShell

Rad sa PowerShell ili skripti u usluzi SharePoint online? Pogledajte dolenavedene veze za više informacija.
- [Prvi koraci uz SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Povezivanje sa SPO PowerShell pomoću verifikacije identiteta (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint obrasci i prakse (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sadrže biblioteku PowerShell komandi koje vam omogućavaju da obavljate komplikovane radnje upravljanja prema SPO.

> [!NOTE]
> - Ako imate problema sa povezivanjem sa SPO Management Shell, uverite se da ste ažurirali najnoviju verziju i pokušajte da [ponovo uvezete modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomoću *"import-modul Microsoft. online. SharePoint. PowerShell".*
> - Ako pokušavate da pokrećete skripte modela sa strane objekta klijenta, moraćete da imate instaliran [SharePoint online Client Components](https://www.microsoft.com/download/details.aspx?id=42038) na lokalnom računaru.
> - Ako imate problema sa pokretanjem skripti iz programa PowerShell, možda biste želeli da razmotrite pokretanje programskog dodatka PowerShell kao administratora i da biste promenili [smernice izvršavanja](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).