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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="ed963-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="ed963-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="ed963-103">Radite sa programom PowerShell ili skriptima u okviru usluge SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="ed963-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="ed963-104">Posetite veze u nastavku da biste dobili više informacija.</span><span class="sxs-lookup"><span data-stu-id="ed963-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="ed963-105">Getting started with SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="ed963-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="ed963-106">Povezivanje sa uslugom SPO PowerShell pomoću višestruke potvrde identiteta (MFA)</span><span class="sxs-lookup"><span data-stu-id="ed963-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="ed963-107">SharePoint obrasci i prakse [(PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sadrži biblioteku PowerShell komandi koja vam omogućava da izvršite složene radnje upravljanja prema SPO- u.</span><span class="sxs-lookup"><span data-stu-id="ed963-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="ed963-108">Ako imate problema sa povezivanjem sa sistemom SPO management shell, [uverite](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) se da ste ažurirali na najnoviju verziju i pokušajte ponovo da uvezete modul pomoću *"Import-Module Microsoft.Online.SharePoint.PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="ed963-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="ed963-109">Ako pokušavate da pokrenete skripte modela objekta na strani klijenta, morate da imate [SDK](https://www.microsoft.com/download/details.aspx?id=42038) za Sharepoint Online klijentske komponente instaliran na lokalnom računaru.</span><span class="sxs-lookup"><span data-stu-id="ed963-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="ed963-110">Ako imate problema sa pokretanjem skripti iz usluge PowerShell, možda ćete želeti da razmotrite pokretanje usluge PowerShell kao administratora i promenu smernica [za izvršavanje.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="ed963-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>