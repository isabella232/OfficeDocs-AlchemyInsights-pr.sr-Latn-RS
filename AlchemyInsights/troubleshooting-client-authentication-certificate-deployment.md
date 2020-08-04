---
title: Rešavanje problema sa primenom certifikata za potvrdu verodostojnosti klijenta
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555811"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="db72c-102">Rešavanje problema sa primenom certifikata za potvrdu verodostojnosti klijenta</span><span class="sxs-lookup"><span data-stu-id="db72c-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="db72c-103">Intune NDES/SCEP i PKCS/PFX profili certifikata se obično koriste zajedno sa drugim tipovima profila kao što su WiFi, VPN i e-pošta da bi korisnicima omogućio identitet korporacijskih resursa.</span><span class="sxs-lookup"><span data-stu-id="db72c-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="db72c-104">Kada su ti tipovi profila povezani sa profilom certifikata klijenta, zavisi od uspešnog raspoređivanja tog profila.</span><span class="sxs-lookup"><span data-stu-id="db72c-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="db72c-105">Početno podešavanje infrastrukture i pridružena konfiguracija profila certifikata klijenta često zahtevaju rešavanje problema.</span><span class="sxs-lookup"><span data-stu-id="db72c-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="db72c-106">Za Postepeni vodič za uspešno podešavanje NDES konektora i uputstva za rešavanje problema za izoliranje problema sa primenom certifikata, pogledajte:</span><span class="sxs-lookup"><span data-stu-id="db72c-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="db72c-107">Konfigurišite infrastrukturu za podršku SCEP sa Intune</span><span class="sxs-lookup"><span data-stu-id="db72c-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="db72c-108">Pregled za Rješavanje problema sa SCEP profilima certifikata pomoću usluge Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="db72c-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="db72c-109">Koristite referentne skripte ljuske da biste proverili konfiguraciju.</span><span class="sxs-lookup"><span data-stu-id="db72c-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="db72c-110">Više informacija potražite u članku [Intune skripte za verifikaciju konektora certifikata](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="db72c-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="db72c-111">**Drugih uobičajenih pitanja**</span><span class="sxs-lookup"><span data-stu-id="db72c-111">**Other common issues**</span></span>

<span data-ttu-id="db72c-112">**Kada pokušam da instaliram priključak za Intune potvrde na server NDES Connector, dobijam poruku "nije moguće proveriti lozinku u zahtevu za certifikat. Možda je već korišćen. Pribavite novu lozinku za prosleđivanje sa ovim zahtevom. "**</span><span class="sxs-lookup"><span data-stu-id="db72c-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="db72c-113">Ova poruka znači da je potrebno da pokrenete instalaciju sa konektorom za certifikat kao administrator.</span><span class="sxs-lookup"><span data-stu-id="db72c-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="db72c-114">U nekim okruženjima, serveri na kojima pokreće Intune certifikat moraju da koriste proxy server za povezivanje sa uslugom Intune, kao i da konektor certifikata mora da koristi proxy.</span><span class="sxs-lookup"><span data-stu-id="db72c-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="db72c-115">U nekim okolnostima, NDES Connector zanemaruje konfigurisane proxy postavke i možda će biti neophodno da konfigurišete postavke proxy servera dok se radi u bezbednosnom kontekstu Localsistema.</span><span class="sxs-lookup"><span data-stu-id="db72c-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="db72c-116">Rešenje je pokretanje programa Internet Explorer kao sistema i konfigurisanje proxy servera u programu IE.</span><span class="sxs-lookup"><span data-stu-id="db72c-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="db72c-117">Nakon ponovnog pokretanja usluge Intune Connector, NDES konektor se povezuje sa Intune.</span><span class="sxs-lookup"><span data-stu-id="db72c-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="db72c-118">**Korisnički uređaji više ne primaju certifikate za SCEP iz NDES.**</span><span class="sxs-lookup"><span data-stu-id="db72c-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="db72c-119">Moguće je da je certifikat za potvrdu identiteta klijenta izdao na NDES server, a naveden za vreme instalacije NDES Connector je istekao ili je nestao.</span><span class="sxs-lookup"><span data-stu-id="db72c-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="db72c-120">Da biste otklonili:</span><span class="sxs-lookup"><span data-stu-id="db72c-120">To resolve:</span></span> 
 
1. <span data-ttu-id="db72c-121">Deinstalirajte NDES konektor.</span><span class="sxs-lookup"><span data-stu-id="db72c-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="db72c-122">Koristite ove detalje da biste zahtevali novu potvrdu identiteta klijenta ili certifikat potvrde identiteta servera:</span><span class="sxs-lookup"><span data-stu-id="db72c-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="db72c-123">Naziv subjekta: CN = spoljašnji FQDN</span><span class="sxs-lookup"><span data-stu-id="db72c-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="db72c-124">Alternativno ime teme (potrebno je oboje): DNS = eksterni FQDN, DNS = interni FQDN</span><span class="sxs-lookup"><span data-stu-id="db72c-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="db72c-125">Ponovo instalirajte NDES Connector sa novim certifikatom.</span><span class="sxs-lookup"><span data-stu-id="db72c-125">Reinstall the NDES connector with the new certificate.</span></span>