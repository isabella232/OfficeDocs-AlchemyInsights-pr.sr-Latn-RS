---
title: Ažurirajte DNS zapise da biste zadržali Veb lokaciju sa trenutnim dobavljačem hostinga
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815799"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="4fd03-102">Ažurirajte DNS zapise da biste zadržali Veb lokaciju sa trenutnim dobavljačem hostinga</span><span class="sxs-lookup"><span data-stu-id="4fd03-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="4fd03-103">U Microsoft 365 centru administracije idite na stranicu **Podešavanje**  >  [domena](https://admin.microsoft.com/Adminportal#/Domains) i na listi domena izaberite domen koji koristite za Veb lokaciju.</span><span class="sxs-lookup"><span data-stu-id="4fd03-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="4fd03-104">Izaberite stavku **+ novi prilagođeni zapis** i unesite sledeće:</span><span class="sxs-lookup"><span data-stu-id="4fd03-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4fd03-105">Za **tip DNS** unesite: **A (adresa)**</span><span class="sxs-lookup"><span data-stu-id="4fd03-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="4fd03-106">Za **ime hosta ili pseudonim**, otkucajte sledeće: **@**</span><span class="sxs-lookup"><span data-stu-id="4fd03-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="4fd03-107">Za **IP adresu**otkucajte STATIČNU IP adresu za Veb lokaciju na kojoj se trenutno nalazi (na primer,: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="4fd03-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="4fd03-108">Ovo mora biti  *statična*  IP adresa za Veb lokaciju, a ne  *dinamična*  IP adresa.</span><span class="sxs-lookup"><span data-stu-id="4fd03-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="4fd03-109">Proverite sa lokacijom na kojoj se vaša Veb lokacija nalazi kako biste se uverili da možete da dobijete statičnu IP adresu za javnu Veb lokaciju.</span><span class="sxs-lookup"><span data-stu-id="4fd03-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="4fd03-110">Izaberite stavku **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="4fd03-110">Select **Save**.</span></span>

<span data-ttu-id="4fd03-111">Pored toga, možete da kreirate CNAME zapis da biste pomogli korisnicima da pronađu Veb lokaciju.</span><span class="sxs-lookup"><span data-stu-id="4fd03-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="4fd03-112">Izaberite stavku **+ novi prilagođeni zapis** i unesite sledeće:</span><span class="sxs-lookup"><span data-stu-id="4fd03-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="4fd03-113">Za **tip DNS** unesite: **CNAME (pseudonim)**</span><span class="sxs-lookup"><span data-stu-id="4fd03-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="4fd03-114">Za **ime hosta ili pseudonim**, otkucajte sledeće: **www**</span><span class="sxs-lookup"><span data-stu-id="4fd03-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="4fd03-115">Za **adresu na adresu**otkucajte potpuno određeno ime domena (FQDN) za Veb lokaciju (na primer, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4fd03-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="4fd03-116">Izaberite stavku **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="4fd03-116">Select **Save**.</span></span>
