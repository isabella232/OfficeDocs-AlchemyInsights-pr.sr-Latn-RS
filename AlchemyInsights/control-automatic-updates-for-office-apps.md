---
title: Kontrolisanje automatskih ispravki za Office aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439923"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="88438-102">Kontrolisanje automatskih ispravki za Office aplikacije</span><span class="sxs-lookup"><span data-stu-id="88438-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="88438-103">Podrazumevano, ispravke za Office aplikacije se preuzimaju automatski i primenjuju u pozadini bez intervencije korisnika.</span><span class="sxs-lookup"><span data-stu-id="88438-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="88438-104">Međutim, administratori mogu da kontrolišu način na koji se ispravke primenjuju pomoću postavki Office Update.</span><span class="sxs-lookup"><span data-stu-id="88438-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="88438-105">Postavke ažuriranja omogućavaju administratorima da omoguće ili onemoguće automatsko ažuriranje, da prikažu ili sakriju dugme " **Ažuriraj odmah** " u sistemu Office, postave rokove ažuriranja i još mnogo toga.</span><span class="sxs-lookup"><span data-stu-id="88438-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="88438-106">Detaljnije informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="88438-106">For detailed information, see:</span></span>

- [<span data-ttu-id="88438-107">Konfigurišite postavke ažuriranja za Office</span><span class="sxs-lookup"><span data-stu-id="88438-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="88438-108">Automatsko ažuriranje za Office nije omogućeno</span><span class="sxs-lookup"><span data-stu-id="88438-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="88438-109">Definišite kako će se Office ažurirati nakon instalacije</span><span class="sxs-lookup"><span data-stu-id="88438-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="88438-110">Da biste redigovali postojeće postavke za ažuriranje primenjene na klijentsku mašinu, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="88438-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="88438-111">Otvorite alatku "Uređivač registratora" tako što ćete **pokrenuti**  >  **Run**  >  **program Regedit**.</span><span class="sxs-lookup"><span data-stu-id="88438-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="88438-112">Prebacite se na sledeću lokaciju i Pregledajte postavke za Office Update:</span><span class="sxs-lookup"><span data-stu-id="88438-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="88438-113">A.</span><span class="sxs-lookup"><span data-stu-id="88438-113">a.</span></span> <span data-ttu-id="88438-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="88438-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="88438-115">B.</span><span class="sxs-lookup"><span data-stu-id="88438-115">b.</span></span> <span data-ttu-id="88438-116">Konplje\konfiguracija</span><span class="sxs-lookup"><span data-stu-id="88438-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="88438-117">**Belešku**  Ako je ključ OfficeMgmtCOM postavljen, možda ćete videti poruku "ispravke kojima upravlja administrator sistema" na **Office**  >  **nalozima Office naloga**  >  **Office Updates**.</span><span class="sxs-lookup"><span data-stu-id="88438-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="88438-118">Više informacija potražite u članku [Upravljanje ispravkama za microsoft 365 aplikacije pomoću upravljača za konfiguraciju krajnje tačke sistema Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="88438-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  