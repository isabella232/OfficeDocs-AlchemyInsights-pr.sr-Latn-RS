---
title: Da li vam je potrebna pomoć sa ograničenjima slanja e-pošte?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836293"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="bb134-102">Da li vam je potrebna pomoć sa ograničenjima slanja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="bb134-102">Need help with email sending limits?</span></span>

<span data-ttu-id="bb134-103">Ispod se nalazi **ograničenja slanja po** dizajnu koja se primenjuju u usluzi.</span><span class="sxs-lookup"><span data-stu-id="bb134-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="bb134-104">Više informacija o ovim ograničenjima dokumentovane su [ovde.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="bb134-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="bb134-105">Da bismo odrazili isporuku nezahtevanih masovnih poruka, primenjujemo ograničenja stope primalaca po korisniku na sve odlazne i **interne poruke.**</span><span class="sxs-lookup"><span data-stu-id="bb134-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="bb134-106">U svim SKU-ovima ovo ograničenje je **10.000 primalaca dnevno.**</span><span class="sxs-lookup"><span data-stu-id="bb134-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="bb134-107">Klijenti koji treba da šalju legitimnu masovnu komercijalnu e-poštu (na primer, bištani klijenata) trebalo bi da koriste nezavisne dobavljače koji su specijalizovani za te usluge.</span><span class="sxs-lookup"><span data-stu-id="bb134-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="bb134-108">Napomi: Kada se dostigne ograničenje za stopu primaoca, poruke iz poštanskog sandučeta nije moguće slati dok broj primalaca poslatih poruka u protekla 24 časa ne padne ispod ograničenja.</span><span class="sxs-lookup"><span data-stu-id="bb134-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="bb134-109">Korisnik neće moći da šalje poruke do tog trenutka.</span><span class="sxs-lookup"><span data-stu-id="bb134-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="bb134-110">Ograničenje brzine **poruke od 30 poruka u minutu** primenjuje se na sve SKU-ove.</span><span class="sxs-lookup"><span data-stu-id="bb134-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="bb134-111">To određuje koliko poruka korisnik može da pošalje sa Exchange Online naloga u navedenom periodu.</span><span class="sxs-lookup"><span data-stu-id="bb134-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="bb134-112">Maksimalan broj primalaca koji su dozvoljeni u poljima **Za, Cc** i Bcc za jednu e-poruku, u svim SKU-ovima, jeste **1000 primalaca.**</span><span class="sxs-lookup"><span data-stu-id="bb134-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="bb134-113">Da biste prilagodili ovo ograničenje, [idite ovde.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="bb134-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
