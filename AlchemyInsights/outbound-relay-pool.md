---
title: Outbound relay pool
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381861"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="16c26-102">Outbound relay pool</span><span class="sxs-lookup"><span data-stu-id="16c26-102">Outbound relay pool</span></span>

<span data-ttu-id="16c26-103">Microsoft pravi neke promene konfiguracije za slanje ili prosleđivanje e-pošte putem Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="16c26-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="16c26-104">Poruke se u određenim scenarijima prosleđene ili se šalju putem Microsoft 365 uz pomoć specijalne relejskog prostore.</span><span class="sxs-lookup"><span data-stu-id="16c26-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="16c26-105">Poruke poslate korišćenjem relejskog grupa mogu da završe u fascikli sa neželjenom poštom primaoca.</span><span class="sxs-lookup"><span data-stu-id="16c26-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="16c26-106">Više informacija potražite u temi o [odlaznom isporuki](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="16c26-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="16c26-107">Da biste izbegli scenario pomoću grupa releja, uverite se da prosleđene/prenete poruke ispunjavaju jedan od sledećih kriterijuma:</span><span class="sxs-lookup"><span data-stu-id="16c26-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="16c26-108">Odlazni pošiljalac je prihvaćeni domen zakuca.</span><span class="sxs-lookup"><span data-stu-id="16c26-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="16c26-109">SPF (SPF) prelazi kada poruka bude u Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="16c26-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="16c26-110">Pošta koju je identifikovao DomainKeys (DKIM) na domenu P2 pošiljaoca prelazi kada poruka dođe do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="16c26-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="16c26-111">Poruke koje ispunjavaju gorenavedeni kriterijum ne šalju se putem grupa releja.</span><span class="sxs-lookup"><span data-stu-id="16c26-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="16c26-112">Ako je MX zapis za domen upućivan na nezavisni ili lokalni server, koristite poboljšano filtriranje da biste se uverili da je SPF provera valjanosti ispravna za dolaznu e-poštu i da biste izbegli slanje e-pošte putem baze podataka.</span><span class="sxs-lookup"><span data-stu-id="16c26-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="16c26-113">**Kako da znamo da li to utiče na nas u prostoru releja?**</span><span class="sxs-lookup"><span data-stu-id="16c26-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="16c26-114">Ako prosleđene ili prenete e-poruke koriste neki od gorenavedenih kriterijuma, poruke se neće preneti putem grupa releja.</span><span class="sxs-lookup"><span data-stu-id="16c26-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="16c26-115">Međutim, ako se poruka pošalje putem grupe releja, IP adresu odlaznog servera je u opsegu 40.95.0.0/16, a ime odlaznog servera uključuje **rly** u imenu.</span><span class="sxs-lookup"><span data-stu-id="16c26-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

