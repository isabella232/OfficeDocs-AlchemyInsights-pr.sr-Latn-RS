---
title: Kreiranje i upravljanje oznakama uređaja ili grupama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731966"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="81307-102">Kreiranje i upravljanje oznakama uređaja ili grupama</span><span class="sxs-lookup"><span data-stu-id="81307-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="81307-103">Dodajte oznake na uređaje da biste kreirali logičku otpornost grupe.</span><span class="sxs-lookup"><span data-stu-id="81307-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="81307-104">Oznake uređaja podržavaju odgovarajuće mapiranje mreže, što vam omogućava da priložite različite oznake kako biste uhvatili kontekst i omogućili dinamičko kreiranje liste kao deo incidenta.</span><span class="sxs-lookup"><span data-stu-id="81307-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="81307-105">Oznake se mogu koristiti kao filter u prikazu liste Uređaji ili za grupisnje uređaja.</span><span class="sxs-lookup"><span data-stu-id="81307-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="81307-106">Dodatne informacije o grupisanju uređaja potražite u [temi Kreiranje oznaka uređaja i upravljanje tim.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="81307-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="81307-107">Oznake možete dodati na uređaje tako što ćete:</span><span class="sxs-lookup"><span data-stu-id="81307-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="81307-108">Korišćenje portala</span><span class="sxs-lookup"><span data-stu-id="81307-108">Using the portal</span></span>

- <span data-ttu-id="81307-109">Postavljanje vrednosti ključa registratora</span><span class="sxs-lookup"><span data-stu-id="81307-109">Setting a registry key value</span></span>
 
<span data-ttu-id="81307-110">**Napomogućeno:** Može da postoji kašnjenje između vremena dodavanja oznake na uređaj i njegove dostupnosti na listi uređaja i stranici uređaja.</span><span class="sxs-lookup"><span data-stu-id="81307-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="81307-111">Da biste dodali oznake uređaja pomoću API-ja, pogledajte [dodavanje ili uklanjanje oznaka uređaja API.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="81307-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="81307-112">Dodavanje i upravljanje oznakama uređaja pomoću portala</span><span class="sxs-lookup"><span data-stu-id="81307-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="81307-113">Izaberite uređaj na koji želite da upravljate oznakama.</span><span class="sxs-lookup"><span data-stu-id="81307-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="81307-114">Uređaj možete izabrati ili potražiti u bilo kom od sledećih prikaza:</span><span class="sxs-lookup"><span data-stu-id="81307-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="81307-115">**Bezbednosne operacije – dashboard** Izaberite ime uređaja iz odeljka Uređaji sa aktivnim obaveštenjima.</span><span class="sxs-lookup"><span data-stu-id="81307-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="81307-116">**Red za obaveštenja –** Izaberite ime uređaja pored ikone uređaja u redu za čekanje za obaveštenja.</span><span class="sxs-lookup"><span data-stu-id="81307-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="81307-117">**Lista uređaja** – Izaberite ime uređaja sa liste uređaja.</span><span class="sxs-lookup"><span data-stu-id="81307-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="81307-118">**Polje za pretragu** – Izaberite stavku Uređaj iz padajućeg menija i unesite ime uređaja.</span><span class="sxs-lookup"><span data-stu-id="81307-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="81307-119">Do stranice sa obaveštenjima možete da odete i preko prikaza datoteke i IP adrese.</span><span class="sxs-lookup"><span data-stu-id="81307-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="81307-120">Izaberite **stavku Upravljanje oznakama** u redu radnji odgovora.</span><span class="sxs-lookup"><span data-stu-id="81307-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="81307-121">Kucanje da biste pronašli ili kreirali oznake.</span><span class="sxs-lookup"><span data-stu-id="81307-121">Type to find or create tags.</span></span>

<span data-ttu-id="81307-122">Oznake se dodaju u prikaz uređaja i odražavaju se na prikazu liste Uređaji.</span><span class="sxs-lookup"><span data-stu-id="81307-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="81307-123">Zatim možete da koristite filter Oznake da biste videli relevantnu listu uređaja.</span><span class="sxs-lookup"><span data-stu-id="81307-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="81307-124">Dodatne informacije potražite u [temi Pravljenje oznaka uređaja i upravljanje upravljanih uređajima.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="81307-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>