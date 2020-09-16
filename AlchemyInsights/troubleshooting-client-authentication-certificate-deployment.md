---
title: Rešavanje problema pri primeni certifikata identiteta klijenta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659000"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="842be-102">Rešavanje problema pri primeni certifikata identiteta klijenta</span><span class="sxs-lookup"><span data-stu-id="842be-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="842be-103">Intune/SCEPS i PKCS/PFX certifikati klijenata se najčešće koriste zajedno sa drugim tipovima profila kao što su WiFi, VPN i e-pošta da bi se korisnicima omogućio da potvrde potvrdu u korporacijske resurse.</span><span class="sxs-lookup"><span data-stu-id="842be-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="842be-104">Kada su ovi tipovi profila povezani sa profilom certifikata klijenta zavise od uspešne primene tog profila.</span><span class="sxs-lookup"><span data-stu-id="842be-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="842be-105">Početna konfiguracija infrastrukture i povezana konfiguracija profila certifikata klijenta često zahtevaju rešavanje problema.</span><span class="sxs-lookup"><span data-stu-id="842be-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="842be-106">Za vodič po koracima za uspešno podešavanje NDES konektora i uputstvo za rešavanje problema da bi se izoliram problemi sa primenom certifikata, pogledajte:</span><span class="sxs-lookup"><span data-stu-id="842be-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="842be-107">Konfigurisanje infrastrukture za podršku pomoću Intune</span><span class="sxs-lookup"><span data-stu-id="842be-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="842be-108">Pregled profila certifikata za rešavanje problema sa Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="842be-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="842be-109">Koristite referentne scenarije da biste potvrdili konfiguraciju.</span><span class="sxs-lookup"><span data-stu-id="842be-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="842be-110">Više informacija potražite u članku [skripte za verifikaciju konektora za verifikovanje certifikata](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="842be-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="842be-111">**Drugi uobičajeni problemi**</span><span class="sxs-lookup"><span data-stu-id="842be-111">**Other common issues**</span></span>

<span data-ttu-id="842be-112">**Kada pokušam da instaliram konektor za potvrdu Intune na server NDES Connector, dobijam poruku "lozinka u zahtevu za certifikat ne može biti proverena. Možda je već korišćen. Nabavite novu lozinku za prosleđivanje sa ovim zahtevom. "**</span><span class="sxs-lookup"><span data-stu-id="842be-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="842be-113">Ova poruka znači da treba da pokrećete instalaciju konektora za certifikat kao administrator.</span><span class="sxs-lookup"><span data-stu-id="842be-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="842be-114">U nekom okruženju, serveri na kojima je pokrenut certifikat Intune mora da koristi proxy server za povezivanje sa Intune tako da konektor za certifikat mora da koristi proxy.</span><span class="sxs-lookup"><span data-stu-id="842be-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="842be-115">U odreрenim okolnostima, NDES konektor zanemaruje podešene proxy postavke i možda će biti potrebno da konfigurišu postavke proxy servera dok su u bezbednosnom kontekstu lokalnog sistema.</span><span class="sxs-lookup"><span data-stu-id="842be-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="842be-116">Rešenje je da pokrećete Internet Explorer kao sistem i konfigurišete proxy u IE.</span><span class="sxs-lookup"><span data-stu-id="842be-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="842be-117">Nakon ponovnog pokretanja usluge sistema Intune Connector, NDES konektor se povezuje sa Intune.</span><span class="sxs-lookup"><span data-stu-id="842be-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="842be-118">**Korisnički uređaji više ne primaju sertifikate iz funkcija NDES.**</span><span class="sxs-lookup"><span data-stu-id="842be-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="842be-119">Moguće je da je certifikat identiteta klijenta izdat NDES serveru i naveden tokom instalacije sistema NDES Connector, istekao ili da nedostaje.</span><span class="sxs-lookup"><span data-stu-id="842be-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="842be-120">Da biste rešili:</span><span class="sxs-lookup"><span data-stu-id="842be-120">To resolve:</span></span> 
 
1. <span data-ttu-id="842be-121">Deinstalirajte NDES Connector.</span><span class="sxs-lookup"><span data-stu-id="842be-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="842be-122">Koristite ove detalje da biste zatražili novu potvrdu identiteta klijenta ili certifikat potvrde identiteta servera:</span><span class="sxs-lookup"><span data-stu-id="842be-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="842be-123">Ime teme: CN = spoljni FQDN</span><span class="sxs-lookup"><span data-stu-id="842be-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="842be-124">Alternativno ime subjekta (oba su potrebna): DNS = eksterni FQDN, DNS = interna FQDN</span><span class="sxs-lookup"><span data-stu-id="842be-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="842be-125">Ponovno instaliranje NDES konektora pomoću novog certifikata.</span><span class="sxs-lookup"><span data-stu-id="842be-125">Reinstall the NDES connector with the new certificate.</span></span>