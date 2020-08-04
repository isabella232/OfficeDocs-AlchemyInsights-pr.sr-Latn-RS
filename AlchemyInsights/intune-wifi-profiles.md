---
title: Intune Wi-Fi profili
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555812"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="b7f47-102">Intune Wi-Fi profili</span><span class="sxs-lookup"><span data-stu-id="b7f47-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="b7f47-103">Uspešna implementacija Wi-Fi povezanosti za klijente MDM zavisi od ispravnog rasporednog profila koji odražava zahteve korporativne Wi-Fi infrastrukture.</span><span class="sxs-lookup"><span data-stu-id="b7f47-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="b7f47-104">Da biste pregledali odgovarajuće postavke za klijentske platforme koje istražujete, pogledajte:</span><span class="sxs-lookup"><span data-stu-id="b7f47-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="b7f47-105">Dodavanje Wi-Fi postavki za uređaje sa operativnim sistemom Android u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b7f47-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="b7f47-106">Dodavanje Wi-Fi postavki za Android Enterprise namenske i potpuno upravljane uređaje u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b7f47-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="b7f47-107">Dodavanje Wi-Fi postavki za iOS i iPadOS uređaje u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b7f47-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="b7f47-108">Dodavanje Wi-Fi postavki za Windows 10 i novije uređaje u Intune</span><span class="sxs-lookup"><span data-stu-id="b7f47-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="b7f47-109">Uvezi Wi-Fi postavke za Windows uređaje u usluzi Intune</span><span class="sxs-lookup"><span data-stu-id="b7f47-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="b7f47-110">**Uobičajenih pitanja**</span><span class="sxs-lookup"><span data-stu-id="b7f47-110">**Common Issues**</span></span>

<span data-ttu-id="b7f47-111">**Raspoređujem Wi-Fi profil koji zavisi od rasporednog certifikata navedenog u Wi-Fi profilu. Međutim, profili konfiguracije pokazuju status greške.**</span><span class="sxs-lookup"><span data-stu-id="b7f47-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="b7f47-112">Proverite da li je uređaj primio certifikat.</span><span class="sxs-lookup"><span data-stu-id="b7f47-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="b7f47-113">U Intune, idite na **sve uređaje** i izaberite uređaj > **Konfiguracija uređaja**.</span><span class="sxs-lookup"><span data-stu-id="b7f47-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="b7f47-114">Proverite da li su svi očekivani profili navedeni i u uspešnom stanju.</span><span class="sxs-lookup"><span data-stu-id="b7f47-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="b7f47-115">Ako imate posredničke certifikate u lancu certifikata, proverite da li su oni raspoređeni na Android uređaje.</span><span class="sxs-lookup"><span data-stu-id="b7f47-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="b7f47-116">Da biste proverili status certifikata, idite na **profil konfiguracije uređaja**  >  **Profiles**  >  **Android srednji ca**  >  **Svojstva**  >  **pouzdani certifikat**.</span><span class="sxs-lookup"><span data-stu-id="b7f47-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="b7f47-117">Ako i dalje budete videli greške, pregledajte procedure i odeljke za rešavanje problema.</span><span class="sxs-lookup"><span data-stu-id="b7f47-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="b7f47-118">Više informacija potražite u članku [pregled za Rješavanje problema sa SCEP profilima certifikata pomoću usluge Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="b7f47-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="b7f47-119">**Na uređaj sam rasporedio Wi-Fi profil. Intune pokazuje da je bila uspešna, ali uređaj se ne povezuje sa Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="b7f47-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="b7f47-120">Uspešan status znači da je Intune uspešno rasporedila profil kao konfigurisan.</span><span class="sxs-lookup"><span data-stu-id="b7f47-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="b7f47-121">Međutim, ove konfiguracije se možda ne podudaraju sa vašim mrežnim i/ili zahtevima za potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="b7f47-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="b7f47-122">Za više detalja o Pokušani vezi, pregledajte evidencije u okviru usluge infrastrukture i potvrde identiteta (na kontroleru Wi-Fi pristupnih tačaka i NPS/radijus server).</span><span class="sxs-lookup"><span data-stu-id="b7f47-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="b7f47-123">Možda ćete morati da radite sa mrežnim infrastrukturnim timom ili sa Wi-Fi dobavljačem nezavisnog proizvođača da biste prikupili i redigovali evidencije.</span><span class="sxs-lookup"><span data-stu-id="b7f47-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>