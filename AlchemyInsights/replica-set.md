---
title: Komplet replika
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714256"
---
# <a name="replica-set"></a><span data-ttu-id="1070c-102">Komplet replika</span><span class="sxs-lookup"><span data-stu-id="1070c-102">Replica set</span></span>

<span data-ttu-id="1070c-103">ASABIRANJE se takođe zove kao upravljani domen.</span><span class="sxs-lookup"><span data-stu-id="1070c-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="1070c-104">To su zapravo dva upravljača domena koja se pokreću i održavaju u okviru pozadine.</span><span class="sxs-lookup"><span data-stu-id="1070c-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="1070c-105">Dva funkcija DCs uključujete jedan glavni centar za centar i jednu replikaciju.</span><span class="sxs-lookup"><span data-stu-id="1070c-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="1070c-106">Rezervna kopija u ADODAJE (kontrolisani domen) je automatizovani proces koji upravlja Azure platformom.</span><span class="sxs-lookup"><span data-stu-id="1070c-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="1070c-107">U slučaju problema sa upravljanim domenom, Azure podrška vam može pomoći pri ponovnom uspostavljanju iz rezervne kopije.</span><span class="sxs-lookup"><span data-stu-id="1070c-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="1070c-108">Pravite svaku repliku skupu u virtuelnoj mreži.</span><span class="sxs-lookup"><span data-stu-id="1070c-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="1070c-109">Svaka virtualna mreža mora da bude u okviru svake druge virtuelne mreže koja je host skupu replika kontrolisanog domena.</span><span class="sxs-lookup"><span data-stu-id="1070c-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="1070c-110">Ova konfiguracija kreira topologiju mreže koja podržava replikaciju direktorijuma.</span><span class="sxs-lookup"><span data-stu-id="1070c-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="1070c-111">Virtuelna mreža može da podrži više skupova replika, pod uslovom da se svaka grupa replika nalazi u drugoj virtualnoj podmreži.</span><span class="sxs-lookup"><span data-stu-id="1070c-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="1070c-112">Za više detalja o skupu replika pogledajte [skupove replika koncepata](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="1070c-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
