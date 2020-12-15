---
title: Uređaj u stanju čekanja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679990"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="730e4-102">Uređaj u stanju čekanja</span><span class="sxs-lookup"><span data-stu-id="730e4-102">Device in pending state</span></span>

<span data-ttu-id="730e4-103">**Preduslovi**</span><span class="sxs-lookup"><span data-stu-id="730e4-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="730e4-104">Ako podešavate registraciju uređaja po prvi put, uverite se da ste redigovali [Uvod u upravljanje uređajima u usluzi Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) koji će vas voditi na način na koji se uređaji mogu kontrolisati u kontroli Azure AD.</span><span class="sxs-lookup"><span data-stu-id="730e4-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="730e4-105">Ako registraciju uređaja u Azure AD registrujete direktno i unosite ih u Intune, moraćete da proverite da li ste prvo [konfigurisali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i da imaju [licenciranje](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="730e4-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="730e4-106">Uverite se da ste ovlašćeni za obavljanje operacija u usluzi Azure AD i lokalnoj REKLAMI.</span><span class="sxs-lookup"><span data-stu-id="730e4-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="730e4-107">Samo globalni administrator u usluzi Azure AD može da upravlja postavkama za registraciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="730e4-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="730e4-108">Pored toga, ako podešavate automatske registracije u lokalnom aktivnom direktorijumu, moraćete da budete administrator aktivnog direktorijuma i AD FS (ako je primenljivo).</span><span class="sxs-lookup"><span data-stu-id="730e4-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="730e4-109">Hibridni Azure AD pridruži se sistemu za registraciju zahteva uređaje za korporativnu mrežu.</span><span class="sxs-lookup"><span data-stu-id="730e4-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="730e4-110">Radi i preko VPN mreže, ali u tome ima nekih problema.</span><span class="sxs-lookup"><span data-stu-id="730e4-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="730e4-111">Čuli smo da klijenti trebaju pomoć za rešavanje problema sa procesom registracije hibridnog Azure AD.</span><span class="sxs-lookup"><span data-stu-id="730e4-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="730e4-112">**Okruženje za potvrdu identiteta u oblaku (pomoću hash sinhronizacije Azure oglasa lozinki ili prosleрenog identiteta)**</span><span class="sxs-lookup"><span data-stu-id="730e4-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="730e4-113">Ovaj tok registracije je poznat i kao "Pridruživanje sastanku".</span><span class="sxs-lookup"><span data-stu-id="730e4-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="730e4-114">Evo šta se dešava tokom procesa registracije:</span><span class="sxs-lookup"><span data-stu-id="730e4-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="730e4-115">Windows 10 otkriva zapis povezivanja usluge (SCP) kada se korisnik prijavi na uređaj.</span><span class="sxs-lookup"><span data-stu-id="730e4-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="730e4-116">Uređaj prvi put pokušava da preuzme informacije o zakupcu iz klijenta u registratoru, [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="730e4-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="730e4-117">Više informacija potražite u članku [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="730e4-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="730e4-118">Ako ne uspe, uređaj komunicira sa lokalnim aktivnim direktorijumom da bi dobio informacije o zakupcu iz SCP.</span><span class="sxs-lookup"><span data-stu-id="730e4-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="730e4-119">Da biste potvrdili SCP, uputite ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="730e4-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="730e4-120">Preporučujemo omogućavanje SCP-a u aktivnom direktorijumu i samo pomoću dodatka za podešavanje početne validacije.</span><span class="sxs-lookup"><span data-stu-id="730e4-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="730e4-121">Windows 10 pokušava da komunicira sa uslugom Azure AD u okviru konteksta sistema da bi se potvrdio na osnovu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="730e4-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="730e4-122">Možete da proverite da li uređaj može da pristupi Microsoft resursima u okviru sistemskog naloga pomoću [skripata za povezivanje registracije uređaja](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="730e4-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="730e4-123">Windows 10 generiše samopotpisani certifikat i skladišti ga ispod objekta računara u lokalnoj aktivnoj fascikli.</span><span class="sxs-lookup"><span data-stu-id="730e4-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="730e4-124">Ovo zahteva liniju vida na kontroler domena.</span><span class="sxs-lookup"><span data-stu-id="730e4-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="730e4-125">Objekat uređaja koji ima certifikat sinhronizovan je sa lokacijom Azure AD putem Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="730e4-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="730e4-126">Ciklus sinhronizacije je podrazumevano svakih 30 minuta, ali to zavisi od konfiguracije Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="730e4-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="730e4-127">Više informacija potražite u [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="730e4-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="730e4-128">U ovoj fazi, trebalo bi da možete da vidite uređaj tema "**Neobrađeno**" u okviru "oљtrica device" Azure portala.</span><span class="sxs-lookup"><span data-stu-id="730e4-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="730e4-129">Na sledećoj prijavi korisnika na Windows 10, registracija će biti dovršena.</span><span class="sxs-lookup"><span data-stu-id="730e4-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="730e4-130">Ako ste na VPN-u i odjavljivanje/prijava prekida vezu ka domenu, možete ručno pokrenuti registraciju.</span><span class="sxs-lookup"><span data-stu-id="730e4-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="730e4-131">Da biste to uradili:</span><span class="sxs-lookup"><span data-stu-id="730e4-131">To do that:</span></span>
    >
    > <span data-ttu-id="730e4-132">Izdaju `dsregcmd /join` lokalno za administratorski odziv ili daljinski pomoću usluge PSExec na računar.</span><span class="sxs-lookup"><span data-stu-id="730e4-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="730e4-133">Na primer: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="730e4-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="730e4-134">Za uobičajene probleme sa sistemom Azure Active Directory, pogledajte [najčešća pitanja o uređajima](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="730e4-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
