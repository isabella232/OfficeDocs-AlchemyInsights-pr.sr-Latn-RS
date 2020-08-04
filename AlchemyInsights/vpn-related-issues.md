---
title: Problemi sa VPN vezom
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555747"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="a5c26-102">Problemi sa VPN vezom</span><span class="sxs-lookup"><span data-stu-id="a5c26-102">VPN related issues</span></span>

<span data-ttu-id="a5c26-103">Uspešna implementacija VPN veze za klijente MDM zavisi od rasporednog profila koji tačno odražava zahteve VPN infrastrukture.</span><span class="sxs-lookup"><span data-stu-id="a5c26-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="a5c26-104">Za odgovarajuće postavke za klijentske platforme koje istražujete, pogledajte:</span><span class="sxs-lookup"><span data-stu-id="a5c26-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="a5c26-105">Postavke Windows 10 i Windows holografskog uređaja za dodavanje VPN veza pomoću funkcije Intune</span><span class="sxs-lookup"><span data-stu-id="a5c26-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="a5c26-106">Dodavanje VPN postavki na iOS i iPadOS uređajima u usluzi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a5c26-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="a5c26-107">Postavke za Android uređaje da biste konfigurisali VPN u Intune</span><span class="sxs-lookup"><span data-stu-id="a5c26-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="a5c26-108">Dodavanje VPN postavki na macOS uređajima u usluzi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a5c26-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="a5c26-109">Ako vaš VPN profil koristi potvrdu identiteta zasnovanu na certifikatu, uverite se da su u uspešno raspoređene osnovne profile certifikata i potvrde identiteta klijenta povezani sa VPN profilom.</span><span class="sxs-lookup"><span data-stu-id="a5c26-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="a5c26-110">**Uobičajenih pitanja**</span><span class="sxs-lookup"><span data-stu-id="a5c26-110">**Common Issues**</span></span>

<span data-ttu-id="a5c26-111">**Na uređaj sam rasporedio VPN profil. Intune pokazuje da je bila uspešna, ali uređaj se ne povezuje sa VPN mrežom.**</span><span class="sxs-lookup"><span data-stu-id="a5c26-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="a5c26-112">Uspešan status znači da je Intune uspešno rasporedila profil kao konfigurisan.</span><span class="sxs-lookup"><span data-stu-id="a5c26-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="a5c26-113">Međutim, ove konfiguracije se možda ne podudaraju sa vašim mrežnim i/ili zahtevima za potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="a5c26-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="a5c26-114">Pregledajte evidencije u usluzi "infrastruktura" i "usluga za potvrdu identiteta" (na VPN serveru i NPS/radijus server) za više detalja o pokušnoj vezi.</span><span class="sxs-lookup"><span data-stu-id="a5c26-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="a5c26-115">Možda ćete morati da radite sa mrežnim infrastrukturnim timom ili VPN dobavljačem nezavisnog proizvođača da biste prikupili i redigovali evidencije.</span><span class="sxs-lookup"><span data-stu-id="a5c26-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="a5c26-116">**Kada podesim prilagođenu VPN za iOS, funkcija VPN aplikacije nije dostupna.**</span><span class="sxs-lookup"><span data-stu-id="a5c26-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="a5c26-117">VPN aplikacija za iOS uređaje u usluzi Intune je trenutno dostupna određenoj listi dobavljača i partnera, koji takođe moraju da ispunjavaju preduslove za certifikat pre konfigurisanja VPN aplikacije po aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="a5c26-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="a5c26-118">Više informacija potražite u članku [Podešavanje virtuelne privatne mreže (VPN) po aplikacijama za iOS/iPadOS uređaje u usluzi Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="a5c26-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="a5c26-119">Za više informacija o svim tipovima VPN veza u usluzi Intune pogledajte odeljak [Kreiranje VPN profila za povezivanje sa VPN serverima u usluzi Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="a5c26-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="a5c26-120">**VPN na zahtev ne pokreće se kada se pristupi konfigurisanim domenom**</span><span class="sxs-lookup"><span data-stu-id="a5c26-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="a5c26-121">Da biste testirali automatsko VPN postavke, postavite sledeće vrednosti:</span><span class="sxs-lookup"><span data-stu-id="a5c26-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="a5c26-122">Želim da uradim sledeće: **procenite svaki pokušaj povezivanja**</span><span class="sxs-lookup"><span data-stu-id="a5c26-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="a5c26-123">Odaberite da li želite da se povežete: **Poveži se ako je potrebno**</span><span class="sxs-lookup"><span data-stu-id="a5c26-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="a5c26-124">Kada korisnici pristupaju ovim domenima: ime **ciljnog** *domena*</span><span class="sxs-lookup"><span data-stu-id="a5c26-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="a5c26-125">Ako gorenavedena Konfiguracija nije uspešna, dodajte sledeći element:</span><span class="sxs-lookup"><span data-stu-id="a5c26-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="a5c26-126">Kada je ova URL adresa nedostupna, Nametni povezivanje VPN-a: **Badurl**</span><span class="sxs-lookup"><span data-stu-id="a5c26-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>