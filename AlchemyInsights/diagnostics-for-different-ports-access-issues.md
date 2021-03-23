---
title: Dijagnoza za različiti problemi sa priključkom na portove
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036810"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="7be2a-102">Dijagnoza za različiti problemi sa priključkom na portove</span><span class="sxs-lookup"><span data-stu-id="7be2a-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="7be2a-103">Da biste rešili drugačiji problem pristupa portova, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="7be2a-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="7be2a-104">Zaustavite/o pronalaženju virtuelnog mašinskog (VR) sa portala, ponovo pokrenite Vim i testirajte ponovo.</span><span class="sxs-lookup"><span data-stu-id="7be2a-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="7be2a-105">Proverite postavke mrežne mreže za VANGOVE osobe da biste utvrdili da li imate mrežne bezbednosne grupe (NSGs) blokiranjem saobraćaja.</span><span class="sxs-lookup"><span data-stu-id="7be2a-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="7be2a-106">Možete da koristite i [alatku verifikovanje IP toka sistema Network posmatrače protoka](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) da biste proverili da li su NSGs blokirali saobraćaj, User-Defined rute (Usus) preusmeravanje saobraćaja nazad na lokalno (' podrazumevani put ' 0.0.0.0/0) ili na mrežni aparat.</span><span class="sxs-lookup"><span data-stu-id="7be2a-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="7be2a-107">Ako i dalje nailazite na probleme posle pokušaja da pokušate da uradite korake iznad, obezbedite ime za Vim i TCP port na koji pokušavate da pošaljete poštu za dalju dijagnozu.</span><span class="sxs-lookup"><span data-stu-id="7be2a-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="7be2a-108">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="7be2a-108">**Recommended Documents**</span></span>

[<span data-ttu-id="7be2a-109">Ograničenja i preporuke za slanje odlazne e-pošte preko porta 25</span><span class="sxs-lookup"><span data-stu-id="7be2a-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)