---
title: SharePoint online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786903"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="c0474-102">SharePoint online PowerShell</span><span class="sxs-lookup"><span data-stu-id="c0474-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="c0474-103">Rad sa PowerShell ili skripti u usluzi SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="c0474-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="c0474-104">Pogledajte dolenavedene veze za više informacija.</span><span class="sxs-lookup"><span data-stu-id="c0474-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="c0474-105">Prvi koraci uz SharePoint online Management Shell</span><span class="sxs-lookup"><span data-stu-id="c0474-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="c0474-106">Povezivanje sa SPO PowerShell pomoću verifikacije identiteta (MFA)</span><span class="sxs-lookup"><span data-stu-id="c0474-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="c0474-107">[SharePoint obrasci i prakse (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sadrže biblioteku PowerShell komandi koje vam omogućavaju da obavljate komplikovane radnje upravljanja prema SPO.</span><span class="sxs-lookup"><span data-stu-id="c0474-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="c0474-108">Ako imate problema sa povezivanjem sa SPO Management Shell, uverite se da ste ažurirali najnoviju verziju i pokušajte da [ponovo uvezete modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) pomoću *"import-modul Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="c0474-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="c0474-109">Ako pokušavate da pokrećete skripte modela sa strane objekta klijenta, moraćete da imate instaliran [SharePoint online Client Components](https://www.microsoft.com/download/details.aspx?id=42038) na lokalnom računaru.</span><span class="sxs-lookup"><span data-stu-id="c0474-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="c0474-110">Ako imate problema sa pokretanjem skripti iz programa PowerShell, možda biste želeli da razmotrite pokretanje programskog dodatka PowerShell kao administratora i da biste promenili [smernice izvršavanja](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="c0474-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>