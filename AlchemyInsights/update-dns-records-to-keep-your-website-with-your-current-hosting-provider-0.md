---
title: Ažuriranje DNS zapisa da bi se zadržao veb sajt sa trenutnim dobavljačem usluge hostinga
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827546"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="cee40-102">Ažuriranje DNS zapisa da bi se zadržao veb sajt sa trenutnim dobavljačem usluge hostinga</span><span class="sxs-lookup"><span data-stu-id="cee40-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="cee40-103">U Microsoft 365 centru administacije idite na stranicu Podešavanje domena i na listi domena izaberite domen koji koristite za   >  [](https://admin.microsoft.com/Adminportal#/Domains) veb lokaciju.</span><span class="sxs-lookup"><span data-stu-id="cee40-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="cee40-104">Izaberite **+ Novi prilagođeni** zapis i unesite sledeće:</span><span class="sxs-lookup"><span data-stu-id="cee40-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="cee40-105">Za **tip DNS unesite:** **A (Adresa)**</span><span class="sxs-lookup"><span data-stu-id="cee40-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="cee40-106">Za **polje Ime hosta ili pseudonim** otkucajte sledeće: **@**</span><span class="sxs-lookup"><span data-stu-id="cee40-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="cee40-107">Za **IP** adresu otkucajte statičnu IP adresu na kojoj se veb lokacija trenutno hostuje (na primer, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="cee40-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="cee40-108">To mora biti  *statička*  IP adresa za veb lokaciju, a ne  *dinamička*  IP adresa.</span><span class="sxs-lookup"><span data-stu-id="cee40-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="cee40-109">Proverite na lokaciji na kojoj se vaša veb lokacija hostuje da biste se uverili da možete da dobijete statičnu IP adresu za javnu veb lokaciju.</span><span class="sxs-lookup"><span data-stu-id="cee40-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="cee40-110">Izaberite **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="cee40-110">Select **Save**.</span></span>

<span data-ttu-id="cee40-111">Pored toga, možete da kreirate CNAME zapis da biste pomogli klijentima da pronađu vašu veb lokaciju.</span><span class="sxs-lookup"><span data-stu-id="cee40-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="cee40-112">Izaberite **+ Novi prilagođeni** zapis i unesite sledeće:</span><span class="sxs-lookup"><span data-stu-id="cee40-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="cee40-113">Za **tip DNS unesite:** **CNAME (pseudonim)**</span><span class="sxs-lookup"><span data-stu-id="cee40-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="cee40-114">Za **polje Ime hosta ili pseudonim** otkucajte sledeće: **www**</span><span class="sxs-lookup"><span data-stu-id="cee40-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="cee40-115">Za **polje Upućuje** na adresu otkucajte potpuno kvalifikovano ime domena (FQDN) za veb lokaciju (na primer, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="cee40-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="cee40-116">Izaberite **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="cee40-116">Select **Save**.</span></span>
