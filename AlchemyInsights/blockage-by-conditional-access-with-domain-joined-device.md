---
title: Blokirano mi je uslovno pristup uz uređaj koji se pridružio domenu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038101"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="757d8-102">Blokirano mi je uslovno pristup uz uređaj koji se pridružio domenu</span><span class="sxs-lookup"><span data-stu-id="757d8-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="757d8-103">**Visoko preporučene alatke**</span><span class="sxs-lookup"><span data-stu-id="757d8-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="757d8-104">[Alatka za rešavanje problema sa registracijom uređaja](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – alatka koja pomaže u rešavanju problema sa najčešćim problemima sa registracijom uređaja.</span><span class="sxs-lookup"><span data-stu-id="757d8-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="757d8-105">[Probna greška registracionog povezivanja uređaja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – scenarij koji pomaže da se osigura da uređaj pristupi krajnjim tačkama registracije uređaja ispod sistemskog naloga.</span><span class="sxs-lookup"><span data-stu-id="757d8-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="757d8-106">[Azure reklama za čišćenje](https://github.com/mzmaili/AzureADDeviceCleanup) -rukopis koji vam omogućava da tražite zastarele uređaje u okruženju i da ih upravljate.</span><span class="sxs-lookup"><span data-stu-id="757d8-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="757d8-107">Evo nekih uobičajenih razloga zbog kojih uslovno pristup možda otkazuje uređaj koji se pridružio domenu (hibridni Azure AD).</span><span class="sxs-lookup"><span data-stu-id="757d8-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="757d8-108">**Ne postoji Azure PRT reklama na uređaju** – morate da se osigurate da uređaj ima Token Azure AD primarno osvežavanje (prt).</span><span class="sxs-lookup"><span data-stu-id="757d8-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="757d8-109">Više informacija o PRT-u potražite u [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="757d8-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="757d8-110">Da biste proverili da li imate Azure AD PRT, možete da pokrećete `dsregcmd/status` komandu na uređaju i proverite da li je "Azučitprt" jednako "da".</span><span class="sxs-lookup"><span data-stu-id="757d8-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="757d8-111">Ako je "Azučitprt" "ne", potvrdite sledeće:</span><span class="sxs-lookup"><span data-stu-id="757d8-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="757d8-112">**Bez obzira na to da li imate federirani ambijent sa uslugom AD FS i nije pristupačan na kućnim mrežama vaših korisnika**: u ovom slučaju, uverite se da su krajnje tačke "razlikovanje korisnika" pristupačne na osnovu ektraneta.</span><span class="sxs-lookup"><span data-stu-id="757d8-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="757d8-113">Ako se oglas bavi za VPN, uverite se da se korisnici povežu sa VPN mrežom i ponovo se prijavite na uređaj.</span><span class="sxs-lookup"><span data-stu-id="757d8-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="757d8-114">Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="757d8-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="757d8-115">**Da li je TPM TPM neispravan i na taj način ne može da potvrdi verodostojnost uređaja**: proverite "TPM. msc" da biste videli da li je stanje TPM "spremno".</span><span class="sxs-lookup"><span data-stu-id="757d8-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="757d8-116">Ako nije, `dsregcmd/leave` Neka se uređaj ponovo pridruži Azure AD.</span><span class="sxs-lookup"><span data-stu-id="757d8-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="757d8-117">Zatim pokušajte ponovo.</span><span class="sxs-lookup"><span data-stu-id="757d8-117">Then, try again.</span></span> <span data-ttu-id="757d8-118">Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="757d8-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="757d8-119">**Koristite nezavisnog dobavljača identiteta, koji ne podržava WS-Trust protokol**.</span><span class="sxs-lookup"><span data-stu-id="757d8-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="757d8-120">Kao što je opisano u našim dokumentima, hibridni Azure spojeni uređaji ne mogu da rade u ovom slučaju.</span><span class="sxs-lookup"><span data-stu-id="757d8-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="757d8-121">Radite sa dobavljačem identiteta za podršku.</span><span class="sxs-lookup"><span data-stu-id="757d8-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="757d8-122">**Korisnici koriste pregledač sa hromom bez Windows 10 naloga** ili **Office proširenja hroma ne koristi automatski prt u udruženim sistemima za AAD ili hibridne AAD**: to dovodi do otkazivanja bilo kakve uslovne smernice zasnovane na uređaju, a prikazuje se poruka o grešci "neregistrovani uređaj".</span><span class="sxs-lookup"><span data-stu-id="757d8-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="757d8-123">Da biste ispravno koristili pregledač sa hromom, morate da instalirate "Windows 10 nalozi" ili "Office ekstenzije za korisnike" putem usluge SCCM ili Intune.</span><span class="sxs-lookup"><span data-stu-id="757d8-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="757d8-124">Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="757d8-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="757d8-125">Ako ne možete da pritisnete daljinski upravljač, obavestite korisnike da ručno instaliraju jednu od gorenavedenih proširenja da biste pristupili aplikacijama koje imaju uslovni pristup zasnovan na uređaju.</span><span class="sxs-lookup"><span data-stu-id="757d8-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="757d8-126">Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="757d8-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="757d8-127">**Uređaj je bio ispravljen hibridni Azuri AD je pridružen, ali je nenamerno izbrisan ili invalid, bilo da su sinhronizovane promene u alatki AZOR AD Connect ili sa azulskog portala**: ako se to desi, objekat sa uređajem se više ne prepoznaje kao potpuno spojeni uređaj, čak i ako je status "Azureadconnect" i "prt" prikazan kao važeće na uređaju.</span><span class="sxs-lookup"><span data-stu-id="757d8-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="757d8-128">Da biste rešili ovaj problem, uradite to `dsregcmd/leave` na uređajima na koje utiče i dozvolite im da se ponovo pridruži Azure AD.</span><span class="sxs-lookup"><span data-stu-id="757d8-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="757d8-129">Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="757d8-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="757d8-130">Ako su uređaji u operativnom sistemu Windows 10, 1809 Update, uz VPN/Cloud proxy i pogledajte probleme sa stanjem "Azučitprt" ili bilo koju aplikaciju sa SSO problemom (Outlook ne povezuje sa poštanskim sandučetom čak i ako ste imali PRT), uverite se da imate ovu zakrpu [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ili aprilske kumulativne ispravke [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) da biste sprečili propusta na tim uređajima.</span><span class="sxs-lookup"><span data-stu-id="757d8-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















