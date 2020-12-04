---
title: Rešavanje problema sa PRT-om
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573725"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="6ec68-102">Rešavanje problema sa PRT-om</span><span class="sxs-lookup"><span data-stu-id="6ec68-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="6ec68-103">Da bi bilo koji uređaj mogao da se dovrši, mora da bude potpuno registrovan i u dobroj državi i da može da pribavi primarni Token osvežavanja (PRT).</span><span class="sxs-lookup"><span data-stu-id="6ec68-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="6ec68-104">Hibridni Azure AD pridruži se sistemu za registraciju zahteva uređaje za korporativnu mrežu.</span><span class="sxs-lookup"><span data-stu-id="6ec68-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="6ec68-105">Radi i preko VPN mreže, ali u tome ima nekih problema.</span><span class="sxs-lookup"><span data-stu-id="6ec68-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="6ec68-106">Čuli smo da klijenti treba da imaju pomoć za rešavanje problema sa operativnim sistemom Azure AD se pridruži registraciji u okviru okolnosti sa udaljenog posla.</span><span class="sxs-lookup"><span data-stu-id="6ec68-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="6ec68-107">Evo šta se dešava, tokom procesa registracije.</span><span class="sxs-lookup"><span data-stu-id="6ec68-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="6ec68-108">**Okruženje za potvrdu identiteta u oblaku (pomoću hash sinhronizacije Azure oglasa lozinki ili prosleрenog identiteta)**</span><span class="sxs-lookup"><span data-stu-id="6ec68-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="6ec68-109">Ovaj tok registracije je poznat i kao "Pridruživanje sastanku".</span><span class="sxs-lookup"><span data-stu-id="6ec68-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="6ec68-110">Windows 10 otkriva SCP zapis po prijavljivanju korisnika na uređaj.</span><span class="sxs-lookup"><span data-stu-id="6ec68-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="6ec68-111">Uređaj prvi put pokušava da preuzme informacije o zakupcu iz klijenta u registratoru, [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="6ec68-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="6ec68-112">Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="6ec68-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="6ec68-113">Ako ne uspe, uređaj komunicira sa lokalnim aktivnim direktorijumom (AD) da biste dobili informacije o zakupcu iz tačaka povezivanja usluge (SCP).</span><span class="sxs-lookup"><span data-stu-id="6ec68-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="6ec68-114">Da biste potvrdili SCP, pogledajte ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="6ec68-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="6ec68-115">Preporučujemo omogućavanje SCP-a u OGLASU i samo pomoću dodatka za početnu validaciju.</span><span class="sxs-lookup"><span data-stu-id="6ec68-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="6ec68-116">Windows 10 pokušava da komunicira sa uslugom Azure AD u okviru konteksta sistema da bi se potvrdio na osnovu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6ec68-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="6ec68-117">Možete da proverite da li uređaj može da pristupi Microsoft resursima u okviru sistemskog naloga pomoću skripata za povezivanje registracije uređaja.</span><span class="sxs-lookup"><span data-stu-id="6ec68-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="6ec68-118">Windows 10 generiše samopotpisani certifikat i skladišti ga ispod objekta računara u lokalnoj REKLAMI.</span><span class="sxs-lookup"><span data-stu-id="6ec68-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="6ec68-119">Ovo zahteva liniju vida na kontroler domena.</span><span class="sxs-lookup"><span data-stu-id="6ec68-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="6ec68-120">Objekat uređaja koji ima certifikat se sinhronizuje na Azure AD u usluzi Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6ec68-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="6ec68-121">Ciklus sinhronizacije je podrazumevano svakih 30 minuta, ali to zavisi od konfiguracije usluge Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6ec68-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="6ec68-122">Za više informacija pogledajte ovaj [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="6ec68-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="6ec68-123">U ovoj fazi, trebalo bi da možete da vidite uređaj tema "Neobrađeno" u okviru "oљtrica device" Azure portala.</span><span class="sxs-lookup"><span data-stu-id="6ec68-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="6ec68-124">Na sledećoj prijavi korisnika na Windows 10, registracija će biti dovršena.</span><span class="sxs-lookup"><span data-stu-id="6ec68-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="6ec68-125">Ako ste na VPN-u, a proces prijavljivanja prekida povezivanje, možete ručno pokrenuti registraciju:</span><span class="sxs-lookup"><span data-stu-id="6ec68-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="6ec68-126">Izdate dsregcmd/JOIN lokalno u okviru odziv administratora ili daljinski pomoću PSExec na PC računaru.</span><span class="sxs-lookup"><span data-stu-id="6ec68-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="6ec68-127">Na primer, PsExec-s \\ win10client01 cmd, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="6ec68-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="6ec68-128">Više detalja o problemima sa hibridom pridruživanja potražite u članku [Rešavanje problema sa uređajima](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="6ec68-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
