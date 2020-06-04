---
title: Ažurirajte DNS zapise da biste zadržali Web lokaciju sa trenutnim dobavljačem hostinga
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665774"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="2745d-102">Ažurirajte DNS zapise da biste zadržali Web lokaciju sa trenutnim dobavljačem hostinga</span><span class="sxs-lookup"><span data-stu-id="2745d-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="2745d-103">U Microsoft 365 admin Center idite na stranicu " **Podešavanje**  >  [domena](https://portal.office.com/adminportal/home#/Domains) " i na listi domena izaberite domen koji koristite za svoju Web lokaciju.</span><span class="sxs-lookup"><span data-stu-id="2745d-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="2745d-104">Izaberite **+ novi prilagođeni zapis** i unesite sledeće:</span><span class="sxs-lookup"><span data-stu-id="2745d-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="2745d-105">Za **DNS tip** ENTER: **A (adresa)**</span><span class="sxs-lookup"><span data-stu-id="2745d-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="2745d-106">Za **ime domaćina ili pseudonim**upišite sledeće:**@**</span><span class="sxs-lookup"><span data-stu-id="2745d-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="2745d-107">Za **IP adresu**otkucajte STATIČNU IP adresu za svoju Web lokaciju na kojoj se trenutno hostuje (na primer, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="2745d-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="2745d-108">Ovo mora da bude *statična* IP adresa za Web lokaciju, a ne *Dinamička* IP adresa.</span><span class="sxs-lookup"><span data-stu-id="2745d-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="2745d-109">Proverite sa lokacijom na kojoj se nalazi vaša Web lokacija da biste se uverili da možete da dobijete statičnu IP adresu za svoju javnu Web lokaciju.</span><span class="sxs-lookup"><span data-stu-id="2745d-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="2745d-110">Kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="2745d-110">Select **Save**.</span></span>

<span data-ttu-id="2745d-111">Pored toga, možete da kreirate zapis CNAME da biste pomogli klijentima da pronađu vašu Web lokaciju.</span><span class="sxs-lookup"><span data-stu-id="2745d-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="2745d-112">Izaberite **+ novi prilagođeni zapis** i unesite sledeće:</span><span class="sxs-lookup"><span data-stu-id="2745d-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="2745d-113">Za **DNS tip** unesite: **CNAME (pseudonim)**</span><span class="sxs-lookup"><span data-stu-id="2745d-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="2745d-114">Za **ime domaćina ili pseudonim**upišite sledeće: **www**</span><span class="sxs-lookup"><span data-stu-id="2745d-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="2745d-115">Da **biste dobili poene za adresu**, otkucajte potpuno kvalifikovano ime domena (FQDN) za vašu Web lokaciju (na primer, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="2745d-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="2745d-116">Kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="2745d-116">Select **Save**.</span></span>
