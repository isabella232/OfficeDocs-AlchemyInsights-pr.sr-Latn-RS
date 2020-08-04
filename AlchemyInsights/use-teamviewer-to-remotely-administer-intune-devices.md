---
title: Korišćenje Timprikazivača za daljinsko upravljanje Intune uređajima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555748"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="60af6-102">Korišćenje Timprikazivača za daljinsko upravljanje Intune uređajima</span><span class="sxs-lookup"><span data-stu-id="60af6-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="60af6-103">Uređaji kojima upravlja Intune mogu da se administriraju daljinski, koristeći [Timviewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="60af6-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="60af6-104">Da biste administrirate Intune pomoću Timprikazivača, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="60af6-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="60af6-105">Počnite tako što ćete dobiti akreditive iz Timprikazivača da biste podesili konektor Timprikazivača na Intune.</span><span class="sxs-lookup"><span data-stu-id="60af6-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="60af6-106">Ovo omogućava administratoru da unese akreditive u korisničkom interfejsu "Timviewer konektor" u okviru uređaja, jednokratna operacija za uspostavljanje veze između Intune i usluge Timviewer.</span><span class="sxs-lookup"><span data-stu-id="60af6-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="60af6-107">**Deo 1: pokretanje sesije sa udaljenim uređajem**</span><span class="sxs-lookup"><span data-stu-id="60af6-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="60af6-108">U okviru stavke **Svi uređaji**izaberite uređaj sa kojim želite da započnete udaljenu sesiju.</span><span class="sxs-lookup"><span data-stu-id="60af6-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="60af6-109">Od **... Više**, izaberite **novu sesiju daljinske pomoći**.</span><span class="sxs-lookup"><span data-stu-id="60af6-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="60af6-110">Izaberite **da** da biste potvrdili da želite da uspostavite udaljenu sesiju.</span><span class="sxs-lookup"><span data-stu-id="60af6-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="60af6-111">Nakon što je usluga Timviewer potvrdila zahtev "pokretanje nove udaljene sesije", videćete opciju da **pokrenete daljinsku pomoć** u okviru detalja okna za pregled (ili, Essentials) za uređaj.</span><span class="sxs-lookup"><span data-stu-id="60af6-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="60af6-112">Izaberite stavku **vidi više** da biste razvili okno i prikazali status daljinske pomoći.</span><span class="sxs-lookup"><span data-stu-id="60af6-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="60af6-113">Izaberite stavku " **Započni udaljenu sesiju** " da biste pokrenuli sesiju na strani administratora.</span><span class="sxs-lookup"><span data-stu-id="60af6-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="60af6-114">Odaberite da preuzmete binarni prikazivač "Timviewer" (Windows) i izaberite stavku " **Pokreni**".</span><span class="sxs-lookup"><span data-stu-id="60af6-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="60af6-115">**Belešku** Možete da zanemarite bilo koju stranicu Web pregledača koja je otvorena na Web lokaciji Timviewer.</span><span class="sxs-lookup"><span data-stu-id="60af6-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="60af6-116">Potvrđuje zahtev za aplikaciju Timviewer da bi se promene na uređaju (samo za Windows).</span><span class="sxs-lookup"><span data-stu-id="60af6-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="60af6-117">Pokreće se aplikacija Timviewer i uključuje kôd sesije za potvrdu verodostojnosti veze sa udaljenim uređajem.</span><span class="sxs-lookup"><span data-stu-id="60af6-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="60af6-118">**Deo 2: uređaj koji je usmeren na udaljenu sesiju**</span><span class="sxs-lookup"><span data-stu-id="60af6-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="60af6-119">Otvorite portal "Intune Company".</span><span class="sxs-lookup"><span data-stu-id="60af6-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="60af6-120">Potražite zastavicu za obaveštenje: "vaš IT administrator zahteva kontrolu nad ovim uređajem za sesiju daljinske pomoći" i izaberite obaveštenje.</span><span class="sxs-lookup"><span data-stu-id="60af6-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="60af6-121">Odaberite da preuzmete aplikaciju Timviewer ili da potvrdite Preuzimanje aplikacije Timviewer iz skladišta aplikacija, a zatim izaberite komandu " **Pokreni**".</span><span class="sxs-lookup"><span data-stu-id="60af6-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="60af6-122">**Belešku** Možete da zanemarite bilo koju stranicu Web pregledača koja je otvorena na Web lokaciji Timviewer.</span><span class="sxs-lookup"><span data-stu-id="60af6-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="60af6-123">Potvrđuje zahtev za aplikaciju Timviewer da bi se promene na uređaju (samo za Windows).</span><span class="sxs-lookup"><span data-stu-id="60af6-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="60af6-124">Pokreće se aplikacija Timviewer i uključuje kôd sesije za potvrdu verodostojnosti veze sa udaljenim uređajem.</span><span class="sxs-lookup"><span data-stu-id="60af6-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="60af6-125">Iskačući meni vas pita da li želite da dozvolite pokretanje sesije.</span><span class="sxs-lookup"><span data-stu-id="60af6-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="60af6-126">**Belešku** Kodovi sesije koje je generisao usluga "Timviewer" predstavljaju samo jednokratno korišćenje.</span><span class="sxs-lookup"><span data-stu-id="60af6-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="60af6-127">Ako izgubite vezu, morate da:</span><span class="sxs-lookup"><span data-stu-id="60af6-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="60af6-128">Zatvorite instancu aplikacije Timviewer na udaljenom uređaju i na admin Workstation.</span><span class="sxs-lookup"><span data-stu-id="60af6-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="60af6-129">Zatvorite portal kompanije na udaljenom uređaju.</span><span class="sxs-lookup"><span data-stu-id="60af6-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="60af6-130">Iniciranje nove "nove sesije daljinske pomoći" sa administratorskog portala.</span><span class="sxs-lookup"><span data-stu-id="60af6-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="60af6-131">Ponovo otvorite portal kompanije na udaljenom uređaju da biste dobili novo obaveštenje.</span><span class="sxs-lookup"><span data-stu-id="60af6-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="60af6-132">Preuzmite i otvorite aplikaciju Timviewer na udaljenom uređaju i u okviru administratorske radne stanice kao što je ranije.</span><span class="sxs-lookup"><span data-stu-id="60af6-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>