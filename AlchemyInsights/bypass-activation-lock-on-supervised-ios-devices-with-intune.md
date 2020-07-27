---
title: Zaobilaženje zaključavanja aktivacije na nadglednim iOS uređajima sa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424214"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="e1ee3-102">Zaobilaženje zaključavanja aktivacije na nadglednim iOS uređajima sa Intune</span><span class="sxs-lookup"><span data-stu-id="e1ee3-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="e1ee3-103">Mogućnost zaobilazi zaključavanja aktivacije na iOS uređajima olakšava oporavak iz scenarija u kojem korisnik omogućava zaključavanje aktivacije na korporativnom uređaju, a zatim napušta preduzeće.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="e1ee3-104">Preliminarna zahteva za zaobilaženje zaključavanja aktivacije uključuju:</span><span class="sxs-lookup"><span data-stu-id="e1ee3-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="e1ee3-105">Uređaj je "nadzirao".</span><span class="sxs-lookup"><span data-stu-id="e1ee3-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="e1ee3-106">Zaključavanje za aktivaciju je uspešno omogućeno uz pomoć smernica ograničenja za iOS uređaja u usluzi Intune.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="e1ee3-107">Pored toga, prilikom zaobilazne zaključavanja aktivacije, trebalo bi da:</span><span class="sxs-lookup"><span data-stu-id="e1ee3-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="e1ee3-108">Fizički poseduje uređaj koji je obrisan.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="e1ee3-109">Kopirajte kôd pre nego što izdate brisanje.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="e1ee3-110">**Napomena:** Kôd za brisanje ne razlikuje velika i mala slova, tako da znakovi "-" nisu neophodni.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="e1ee3-111">Više informacija potražite [u članku zaobilaženje zaključavanja aktivacije na nadglednim iOS uređajima sa Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="e1ee3-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="e1ee3-112">**NAJČEŠĆA PITANJA**</span><span class="sxs-lookup"><span data-stu-id="e1ee3-112">**FAQ**</span></span>

<span data-ttu-id="e1ee3-113">Q: **izdao sam udaljenu radnju da biste uklonili podatke o preduzeću sa uređaja, a sada je zaglavljeno u stanju čekanja.**</span><span class="sxs-lookup"><span data-stu-id="e1ee3-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="e1ee3-114">A: da bi se udaljena radnja uspešno dovršila, ciljni uređaj mora biti na mreži i zdrav.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="e1ee3-115">U sledećim situacijama, udaljena radnja ostaje u stanju čekanja 30 dana, ili dok uređaj ne bude priznao komandu kada uređaj:</span><span class="sxs-lookup"><span data-stu-id="e1ee3-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="e1ee3-116">Nema vezu.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-116">Does not have connectivity.</span></span>
- <span data-ttu-id="e1ee3-117">Gubi svoj status upravljanja sa Intune.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="e1ee3-118">Ako mislite da se uređaj više ne proverava i da neće ukloniti podatke o preduzeću, kliknite na dugme "Izbriši".</span><span class="sxs-lookup"><span data-stu-id="e1ee3-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="e1ee3-119">Brisanje uklanja zapis uređaja tako da se više ne pojavljuje na listi za Intune uređaja.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="e1ee3-120">Da bi uređaj ponovo postao aktivan, korisnik mora ponovo da upiše uređaj.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="e1ee3-121">Q: **Zašto određene udaljene radnje nisu dostupne da bi se koristila?**</span><span class="sxs-lookup"><span data-stu-id="e1ee3-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="e1ee3-122">A: ne podržavaju sve platforme sve radnje udaljenog uređaja.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="e1ee3-123">Sledeće udaljene radnje su specifična za platformu.</span><span class="sxs-lookup"><span data-stu-id="e1ee3-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="e1ee3-124">Zaobiđi zaključavanje aktivacije (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="e1ee3-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="e1ee3-125">Novi početak (samo za Windows)</span><span class="sxs-lookup"><span data-stu-id="e1ee3-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="e1ee3-126">Izgubljeni režim (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="e1ee3-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="e1ee3-127">Lociranje uređaja (samo iOS)</span><span class="sxs-lookup"><span data-stu-id="e1ee3-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="e1ee3-128">Ponovo pokreni (samo za Windows)</span><span class="sxs-lookup"><span data-stu-id="e1ee3-128">Restart (Windows only)</span></span>

<span data-ttu-id="e1ee3-129">Više detalja o svakoj radnji potražite u članku [Dostupne radnje uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="e1ee3-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>