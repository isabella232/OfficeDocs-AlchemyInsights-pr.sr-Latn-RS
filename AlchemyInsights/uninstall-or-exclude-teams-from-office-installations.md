---
title: Deinstalacija ili isključite Teams iz Office instalacija
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
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827806"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="77a55-102">Deinstalacija ili isključivanje teams iz novih ili postojećih Office instalacija</span><span class="sxs-lookup"><span data-stu-id="77a55-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="77a55-103">Microsoft Teams je uključen u Microsoft 365 aplikacije za velika preduzeća, Microsoft 365 aplikacije za preduzeća i Office za Mac.</span><span class="sxs-lookup"><span data-stu-id="77a55-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="77a55-104">Koristite [alatku za primenu programskog paketa](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) Office da biste izuzeli Teams iz novih instalacija sistema Office.</span><span class="sxs-lookup"><span data-stu-id="77a55-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="77a55-105">Da *biste deinstalacija aplikacije* Teams sa uređaja sa operativnim sistemom Windows, pogledajte članak [Deinstalacija usluge Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="77a55-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="77a55-106">Da biste očistili Microsoft Teams sa više ciljnih računara ili korisnika, pogledajte članak [Čišćenje Microsoft Teams primene.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="77a55-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="77a55-107">Koristite [opciju "PreventTeamsInstall"](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) da biste sprečili Microsoft Teams da se automatski instalira sa sistemom Office.</span><span class="sxs-lookup"><span data-stu-id="77a55-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="77a55-108">Koristite [opciju PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) pre instaliranja usluge *Teams* kako biste sprečili Microsoft Teams da se automatski pokreće nakon instalacije.</span><span class="sxs-lookup"><span data-stu-id="77a55-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="77a55-109">Ako koristite Office za Mac, pogledajte [članak Microsoft Teams instalacije na Mac računaru.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="77a55-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>