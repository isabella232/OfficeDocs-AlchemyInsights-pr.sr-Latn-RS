---
title: Primena Microsoft 365 aplikacija za preduzeća za zajedničku upotrebu na RDS, Terminal serveru ili VANDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200687"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="b8b63-102">Primena Microsoft 365 aplikacija za preduzeća za zajedničku upotrebu na RDS, Terminal serveru ili VANDI</span><span class="sxs-lookup"><span data-stu-id="b8b63-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="b8b63-103">Da biste primenili Microsoft 365 aplikacije za Enterprise pomoću usluga udaljenog računara (RDS), nekada nazvane usluge terminala:</span><span class="sxs-lookup"><span data-stu-id="b8b63-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="b8b63-104">Morate da imate Microsoft 365 za posao plan ili Office 365 plan koji uključuje Microsoft 365 aplikacije za Enterprise, kao što je Office 365 Enterprise E3 ili Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="b8b63-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="b8b63-105">Microsoft 365 aplikacije za preduzeća i Microsoft 365 poslovni planovi ne uključujući Microsoft 365 aplikacije za Enterprise.</span><span class="sxs-lookup"><span data-stu-id="b8b63-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="b8b63-106">Morate omogućiti [Aktiviranje deljene računara](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="b8b63-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="b8b63-107">Takođe možete da preuzmete i uradite [Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA_OfficeSCA_M365Portal) da biste instalirali Microsoft 365 aplikacije za Enterprise u režimu izvršavanja deljenog računara.</span><span class="sxs-lookup"><span data-stu-id="b8b63-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="b8b63-108">Više informacija o preduslovima, uputstvima za podešavanje i smernicama za prilagođene instalacije pomoću alatke za primenu sistema Office potražite u članku [Primena Microsoft 365 aplikacija za preduzeća pomoću usluga udaljenog računara](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="b8b63-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="b8b63-109">Da biste rešili greške u vezi sa aktivacijom deljenog računara:</span><span class="sxs-lookup"><span data-stu-id="b8b63-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="b8b63-110">Pogledajte članak [Rešavanje problema sa aktivacijom deljenog računara za Microsoft 365 aplikacije za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="b8b63-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="b8b63-111">Pogledajte članak [Resetovanje stanja aktivacije usluge Microsoft 365 Apps za preduzeće](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="b8b63-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="b8b63-112">Ako želite da instalirate Microsoft 365 aplikacije za Enterprise na sajtu RDS iz Microsoft 365 centra administracije, ***koje koristi podrazumevane postavke instalacije***, koristite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="b8b63-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="b8b63-113">Potvrdite koju pretplatu imate.</span><span class="sxs-lookup"><span data-stu-id="b8b63-113">Check what subscription you have.</span></span> <span data-ttu-id="b8b63-114">[Saznajte kako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="b8b63-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="b8b63-115">Ako je potrebno, prebacite se na drugačiju pretplatu.</span><span class="sxs-lookup"><span data-stu-id="b8b63-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="b8b63-116">[Saznajte kako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="b8b63-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="b8b63-117">Ako je Office već instaliran na RDS serveru pomoću drugih Microsoft pretplata, deinstalirajte ga.</span><span class="sxs-lookup"><span data-stu-id="b8b63-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="b8b63-118">Na primer, tako što ćete otići na **kontrolnu tablu** za  >  **Deinstaliranje programa**.</span><span class="sxs-lookup"><span data-stu-id="b8b63-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="b8b63-119">Deinstalirajte pomoću [Microsoft pomoćnika za podršku i oporavak](https://aka.ms/SARA-OfficeUninstall-Alchemy) Ako nailazite na probleme.</span><span class="sxs-lookup"><span data-stu-id="b8b63-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="b8b63-120">Na RDS serveru, prijavite se u Microsoft 365 centar administracije pomoću administratorskog naloga i [instalirajte Microsoft 365 aplikacije za Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="b8b63-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="b8b63-121">Kada se Office instalira, ***Nemojte otvarati ili se prijavljivanjem*** u bilo koju Office aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="b8b63-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="b8b63-122">Na RDS serveru, omogućite aktiviranje deljenog računara uređivanjem registratora tako što ćete pratiti ove korake:</span><span class="sxs-lookup"><span data-stu-id="b8b63-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="b8b63-123">Kliknite desnim tasterom miša na dugme Windows u donjem levom uglu ekrana i izaberite stavku **pokrene**.</span><span class="sxs-lookup"><span data-stu-id="b8b63-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="b8b63-124">U polju otvori otkucajte alatku **rigedit**, a zatim kliknite na **dugme u redu**.</span><span class="sxs-lookup"><span data-stu-id="b8b63-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="b8b63-125">Kliknite na dugme **da** kada vam bude zatraženo da omogućite uređivaču registratora da napravi promene na uređaju.</span><span class="sxs-lookup"><span data-stu-id="b8b63-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="b8b63-126">U uređivaču registratora Dodajte vrednost niske **Sharedkompjuterlicenciranja** sa podešavanjem 1 u okviru HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\clicktorun\url konfiguracione.</span><span class="sxs-lookup"><span data-stu-id="b8b63-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="b8b63-127">Na RDS serveru, ***Prijavite se kao krajnji korisnik*** i [Proverite da li je aktivacija deljenog računara omogućena za Microsoft 365 aplikacije za Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="b8b63-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
