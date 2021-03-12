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
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709084"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="15697-102">SharePoint online PowerShell</span><span class="sxs-lookup"><span data-stu-id="15697-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="15697-103">Rad sa PowerShell ili skripti u usluzi SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="15697-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="15697-104">Pogledajte dolenavedene veze za više informacija.</span><span class="sxs-lookup"><span data-stu-id="15697-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="15697-105">Prvi koraci uz SharePoint online Management Shell</span><span class="sxs-lookup"><span data-stu-id="15697-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="15697-106">Povezivanje sa SPO PowerShell pomoću verifikacije identiteta (MFA)</span><span class="sxs-lookup"><span data-stu-id="15697-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="15697-107">[SharePoint obrasci i prakse (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sadrže biblioteku PowerShell komandi koje vam omogućavaju da obavljate komplikovane radnje upravljanja prema SPO.</span><span class="sxs-lookup"><span data-stu-id="15697-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="15697-108">Ako imate problema sa povezivanjem sa SPO Management Shell, uverite se da ste ažurirali najnoviju verziju i pokušajte da [ponovo uvezete modul](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) pomoću *"import-modul Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="15697-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="15697-109">Ako pokušavate da pokrećete skripte modela sa strane objekta klijenta, moraćete da imate instaliran [SharePoint online Client Components](https://www.microsoft.com/download/details.aspx?id=42038) na lokalnom računaru.</span><span class="sxs-lookup"><span data-stu-id="15697-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="15697-110">Ako imate problema sa pokretanjem skripti iz programa PowerShell, možda biste želeli da razmotrite pokretanje programskog dodatka PowerShell kao administratora i da biste promenili [smernice izvršavanja](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="15697-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>