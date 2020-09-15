---
title: Instaliranje sistema Office na Terminal serveru – nelicencirani
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663131"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="dd5b3-102">Instaliranje sistema Office na Terminal serveru</span><span class="sxs-lookup"><span data-stu-id="dd5b3-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="dd5b3-103">Za primenu Microsoft 365 aplikacija za Enterprise na Windows serveru pomoću usluga udaljenog računara (RDS), nekadašnjih imena usluga terminala:</span><span class="sxs-lookup"><span data-stu-id="dd5b3-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="dd5b3-104">Morate da imate Microsoft 365 pretplatu koja obuhvata Microsoft 365 aplikacije za Enterprise, kao što je Office 365 Enterprise E3 ili Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="dd5b3-105">Microsoft 365 aplikacije za preduzeća i Microsoft 365 aplikacije za preduzeća Premium ne uključujete Microsoft 365 aplikacije za Enterprise.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="dd5b3-106">Treba da omogućite [aktivaciju deljene računara](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="dd5b3-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="dd5b3-107">Ako želite da instalirate Microsoft 365 aplikacije za Enterprise na sajtu RDS iz Microsoft 365 centra administracije, ***koje koriste podrazumevane postavke instalacije***, koristite sledeće korake.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="dd5b3-108">Takođe možete da preuzmete i uradite [Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Microsoft 365 aplikacije za Enterprise u režimu izvršavanja deljenog računara.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="dd5b3-109">Potvrdite koje Microsoft 365 imate.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="dd5b3-110">Saznajte kako</span><span class="sxs-lookup"><span data-stu-id="dd5b3-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="dd5b3-111">Ako je potrebno, prebacite se na neku drugoj Microsoft 365 pretplatu.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="dd5b3-112">Saznajte kako</span><span class="sxs-lookup"><span data-stu-id="dd5b3-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="dd5b3-113">Ako je Office već instaliran na RDS serveru pomoću drugih Microsoft 365 pretplata, deinstalirajte je.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="dd5b3-114">Na primer, tako što ćete otići na kontrolnu tablu za \> Deinstaliranje programa.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="dd5b3-115">Deinstalirajte pomoću [Microsoft pomoćnika za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) Ako nailazite na probleme.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="dd5b3-116">Na RDS serveru, prijavite se u Microsoft 365 centar administracije pomoću administratorskog naloga i [instalirajte Microsoft 365 aplikacije za Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="dd5b3-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="dd5b3-117">Kada se Office instalira, ***Nemojte otvarati ili se prijavljivanjem*** u bilo koju Office aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="dd5b3-118">Na RDS serveru, omogućite aktiviranje deljenog računara uređivanjem registratora tako što ćete pratiti ove korake:</span><span class="sxs-lookup"><span data-stu-id="dd5b3-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="dd5b3-119">Kliknite desnim tasterom miša na dugme Windows u donjem levom uglu ekrana i izaberite stavku pokrene.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="dd5b3-120">U polju otvori otkucajte alatku **rigedit**, a zatim kliknite na dugme u redu.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="dd5b3-121">Kliknite na dugme da kada vam bude zatraženo da omogućite uređivaču registratora da napravi promene na uređaju.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="dd5b3-122">U uređivaču registratora Dodajte vrednost niske **Sharedkompjuterlicenciranja** sa podešavanjem 1 u okviru HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\clicktorun\url konfiguracione.</span><span class="sxs-lookup"><span data-stu-id="dd5b3-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="dd5b3-123">Na RDS serveru, ***Prijavite se kao krajnji korisnik*** i [Proverite da li je aktivacija deljenog računara omogućena za Microsoft 365 aplikacije za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="dd5b3-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="dd5b3-124">Za više detalja o preduslove, uputstva za podešavanje i uputstvo za prilagođene instalacije pomoću alatke za primenu sistema Office pogledajte članak [Primena Microsoft 365 aplikacija za Enterprise pomoću usluga udaljenog računara](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="dd5b3-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="dd5b3-125">Da biste rešili greške u vezi sa aktivacijom deljenog računara, pogledajte članak [Rešavanje problema sa aktivacijom deljenih računara za Microsoft 365 aplikacije za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="dd5b3-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  