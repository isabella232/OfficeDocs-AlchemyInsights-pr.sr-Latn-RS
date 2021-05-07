---
title: Primena programski dodatak za Microsoft 365 aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233548"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="8a5a9-102">Primena programski dodatak za Microsoft 365 aplikacije</span><span class="sxs-lookup"><span data-stu-id="8a5a9-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="8a5a9-103">Centralizovana primena je preporučeni način za primenu Kancelarija za korisnike i grupe u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="8a5a9-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="8a5a9-104">Da biste primenili programski dodatak, pratite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="8a5a9-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="8a5a9-105">**Napomogućeno:** Da biste instalirali programske Kancelarija kao pojedinačni korisnik, pogledajte prikaz programskih dodatak, upravljanje i instaliranje programskih dodatak u [Kancelarija programima.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="8a5a9-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="8a5a9-106">Takođe se uverite da je omogućena pojedinačna Kancelarija prodavnice programski dodaci.</span><span class="sxs-lookup"><span data-stu-id="8a5a9-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="8a5a9-107">Za detalje pogledajte [sprečavanje preuzimanja programski](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)dodataka tako što Kancelarija prodavnicu Store za sve klijente (osim Outlook) .</span><span class="sxs-lookup"><span data-stu-id="8a5a9-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="8a5a9-108">Uverite se da okruženje ispunjava zahteve za primenu programski dodatka pomoću centralizovane primene.</span><span class="sxs-lookup"><span data-stu-id="8a5a9-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="8a5a9-109">Za detalje pogledajte [Zahtevi.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="8a5a9-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="8a5a9-110">Idite na **Postavke** integrisane aplikacije Nabavite aplikacije u Microsoft 365 centra za  >    >   administaciju da biste primenili programski dodatak.</span><span class="sxs-lookup"><span data-stu-id="8a5a9-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="8a5a9-111">Napomene:</span><span class="sxs-lookup"><span data-stu-id="8a5a9-111">Notes:</span></span> 

- <span data-ttu-id="8a5a9-112">Integrisane aplikacije zahtevaju da korisnik ima dozvole globalnog Exchange ili da Exchange za adminitre.</span><span class="sxs-lookup"><span data-stu-id="8a5a9-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="8a5a9-113">Prilikom primene programskih dodatak za više korisnika, preporučujemo da dodele donose pomoću grupa umesto pojedinačnih korisnika.</span><span class="sxs-lookup"><span data-stu-id="8a5a9-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="8a5a9-114">Za detalje pogledajte [razmatranja prilikom dodele programskih dodatka korisnicima i grupama.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="8a5a9-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="8a5a9-115">Centralizovana primena ne podržava korisnike u ugnežđenim grupama ili grupama koje imaju nadređene grupe.</span><span class="sxs-lookup"><span data-stu-id="8a5a9-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="8a5a9-116">Za detalje pogledajte [dodele za korisnika i grupu.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="8a5a9-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="8a5a9-117">Uverite se da je Microsoft 365 Usluga za upravljanje aplikacijama (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') omogućena korisnicima da se prijave.</span><span class="sxs-lookup"><span data-stu-id="8a5a9-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="8a5a9-118">Za detalje pogledajte Konfigurisanje [svojstava aplikacije.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="8a5a9-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="8a5a9-119">Ako naižete na probleme sa primenu programski dodatka pomoću integrisanih aplikacija, pokušajte da primenite [koristeći programski dodatak.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="8a5a9-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="8a5a9-120">Za više informacija pogledajte:</span><span class="sxs-lookup"><span data-stu-id="8a5a9-120">For more information, see:</span></span>

<span data-ttu-id="8a5a9-121">[Primena programskog dodatka u centru za administvene programe](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Upravljanje programski dodacima u centru aktivnosti](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Koristite PowerShell cmdlet cmdlet za centralizovanu primenu za upravljanje programski dodacima](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Objavljivanje Kancelarija korišćenjem centralizovane primene putem Microsoft 365 centra administracije](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Rešavanje problema: Korisnik ne vidi programski dodatak](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Rešavanje problema sa greškama korisnika Kancelarija programski dodaci](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="8a5a9-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>