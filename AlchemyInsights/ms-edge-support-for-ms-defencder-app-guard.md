---
title: Podrška za Microsoft Defender za čuvara aplikacije Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584012"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="c4f9f-102">Podrška za Microsoft Defender za čuvara aplikacije Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="c4f9f-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="c4f9f-103">Dizajnirano za Windows 10 i Microsoft Edge, Gardiska aplikacija koristi hardver-izolacioni pristup koji korisniku omogućava da se kreće na nepouzdani sajt iz izolovanog, hiper-V-omogućenog kontejnera, odvojen od sistema domaćina.</span><span class="sxs-lookup"><span data-stu-id="c4f9f-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="c4f9f-104">Administrativni administrator definiše listu pouzdanih Veb lokacija, resursa oblaka i unutrašnjih mreža.</span><span class="sxs-lookup"><span data-stu-id="c4f9f-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="c4f9f-105">Kada korisnik poseti lokaciju koja nije na listi, Microsoft Edge će otvoriti lokaciju u kontejneru.</span><span class="sxs-lookup"><span data-stu-id="c4f9f-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="c4f9f-106">To znači da ako se ispostavi da je lokacija zlonamerna, računar host će ostati zaštićen i da napadač neće doći do Enterprise podataka.</span><span class="sxs-lookup"><span data-stu-id="c4f9f-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="c4f9f-107">Instalacija proširenja u kontejneru je podržana kao Microsoft Edge verzija 81 i može se kontrolisati pomoću smernica.</span><span class="sxs-lookup"><span data-stu-id="c4f9f-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="c4f9f-108">Adresa Updateula koja se koristi u smernicama za proširive smernice treba da se doda kao neutralan resurs u smernicama za izolaciju mreže koju koristi čuvar aplikacije.</span><span class="sxs-lookup"><span data-stu-id="c4f9f-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="c4f9f-109">Više informacija potražite u članku [Podrška za Microsoft Edge za gardu aplikacije Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="c4f9f-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
