---
title: Pomoć za podešavanje noćnog ekrana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405179"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="31bf6-102">Pomoć za podešavanje noćnog ekrana</span><span class="sxs-lookup"><span data-stu-id="31bf6-102">Help with the night light display setting</span></span>

<span data-ttu-id="31bf6-103">Da biste saznali više o postavkama za noćni ekran, pogledajte [postavljanje ekrana za noćno vreme u operativnom sistemu Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="31bf6-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="31bf6-104">Ako su opcije noćnog svetla zasivo u vašoj postavki, proverite upravljački program ekrana:</span><span class="sxs-lookup"><span data-stu-id="31bf6-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="31bf6-105">Kliknite na polje za pretragu na traci zadataka i ukucajte **Upravljač uređajima**, a zatim u rezultatima **pretrage izaberite** stavku Upravljač uređajima.</span><span class="sxs-lookup"><span data-stu-id="31bf6-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="31bf6-106">Razvijte **video adaptere**.</span><span class="sxs-lookup"><span data-stu-id="31bf6-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="31bf6-107">Nažalost, funkcija noćnog svetla nije dostupna ako uređaj koristi DisplayLink upravljački program ili upravljački program za osnovni prikaz.</span><span class="sxs-lookup"><span data-stu-id="31bf6-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="31bf6-108">Funkcija noćnog svetla koristi nedavne grafičke tehnologije, tako da ćete možda morati da ažurirate upravljački program ekrana:</span><span class="sxs-lookup"><span data-stu-id="31bf6-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="31bf6-109">Proverite da li postoje ispravke tako što ćete **ići na**  >  **početni ekran Postavke**  >  **ažuriranja &**  >  **Ispravke za Windows Update**  >  .</span><span class="sxs-lookup"><span data-stu-id="31bf6-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="31bf6-110">ILI</span><span class="sxs-lookup"><span data-stu-id="31bf6-110">OR</span></span>

- <span data-ttu-id="31bf6-111">Posetite veb lokaciju podrške proizvođača hardvera da biste ručno preuzeli i instalirali najnovije upravljačke programe za prikaz.</span><span class="sxs-lookup"><span data-stu-id="31bf6-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="31bf6-112">Resetuj noćno svetlo u registratoru</span><span class="sxs-lookup"><span data-stu-id="31bf6-112">Reset night light in the registry</span></span>

<span data-ttu-id="31bf6-113">Ako ažuriranje upravljačkog programa za ekran nije uspelo, možda ćete morati da uspostavite početne vrednosti noćnog svetla u registratoru.</span><span class="sxs-lookup"><span data-stu-id="31bf6-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="31bf6-114">**Oprez:** Ovaj korak za rešavanje problema preporučuje se samo za napredne korisnike.</span><span class="sxs-lookup"><span data-stu-id="31bf6-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="31bf6-115">Ako neispravno izmenite registrator, može doći do ozbiljnih problema.</span><span class="sxs-lookup"><span data-stu-id="31bf6-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="31bf6-116">Radi dodatne zaštite, izađite iz rezervne kopije registratora pre nego što ga izmenite kako biste mogli da ga vratite ako dođe do problema.</span><span class="sxs-lookup"><span data-stu-id="31bf6-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="31bf6-117">U polju za pretragu otkucajte **regedit**, a zatim u rezultatima pretrage izaberite **stavku** Uređivač registratora.</span><span class="sxs-lookup"><span data-stu-id="31bf6-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="31bf6-118">Idite na sledeći ključ registratora:</span><span class="sxs-lookup"><span data-stu-id="31bf6-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="31bf6-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="31bf6-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="31bf6-120">Izvezite i izbrišite sledeći potključ:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="31bf6-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="31bf6-121">Izvezite i izbrišite sledeći potključ:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="31bf6-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="31bf6-122">Ponovo pokrenite Windows i proverite da li su dostupne opcije noćnog svetla.</span><span class="sxs-lookup"><span data-stu-id="31bf6-122">Restart Windows and verify if the night light options are available.</span></span>


