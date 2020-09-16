---
title: 1336 fascikla "stavke".
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741281"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="cfdc6-102">Fascikla "stavke koja se može spasti" je popunjena</span><span class="sxs-lookup"><span data-stu-id="cfdc6-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="cfdc6-103">Za Exchange online Poštanske sandučiće, podrazumevano ograničenje prostora za skladištenje stavki je 30 GB.</span><span class="sxs-lookup"><span data-stu-id="cfdc6-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="cfdc6-104">Ograničenje skladišta za fasciklu "stavke koje se mogu spasti" automatski se povećava na 100 GB ako je poštansko sanduče postavljeno na čekanje, eDiscovery ili se dodeljuje smernicama za zadržavanje.</span><span class="sxs-lookup"><span data-stu-id="cfdc6-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="cfdc6-105">Kada fascikla "Oporune stavke" dostigne ograničenje skladišta, funkcionalnost poštanskog sandučeta utiče na sledeće načine:</span><span class="sxs-lookup"><span data-stu-id="cfdc6-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="cfdc6-106">Korisnik ne može da izbriše stavke iz poštanskog sandučeta.</span><span class="sxs-lookup"><span data-stu-id="cfdc6-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="cfdc6-107">Pomoćnik kontrolisane fascikle ne može da izbriše stavke na osnovu postavki za zadržavanje ili kontrolisane fascikle.</span><span class="sxs-lookup"><span data-stu-id="cfdc6-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="cfdc6-108">Za Poštanske sandučiće sa omogućenim oporavkom za oporavak stavki ili se stavljaju na čekanje, proces zaštite stranice kopiranja i pisanja ne može da održi verzije stavki koje uređuje korisnik.</span><span class="sxs-lookup"><span data-stu-id="cfdc6-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="cfdc6-109">Za Poštanske sandučiće sa omogućenim evidentiranju nadzora poštanskog sandučeta, ne mogu se sačuvati datoteke evidencije nadzora u prijemnom poštanskom sandučetu u fascikli "stavke koje se mogu spasti".</span><span class="sxs-lookup"><span data-stu-id="cfdc6-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="cfdc6-110">Za Poštanske sandučiće koji nisu na čekanju, administratori mogu da koriste `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandu u usluzi Exchange online PowerShell za brisanje stavki u fascikli "stavke koje se mogu spasti".</span><span class="sxs-lookup"><span data-stu-id="cfdc6-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="cfdc6-111">Više informacija potražite u sledećim temama:</span><span class="sxs-lookup"><span data-stu-id="cfdc6-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="cfdc6-112">Pretraga i brisanje poruka</span><span class="sxs-lookup"><span data-stu-id="cfdc6-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="cfdc6-113">Pretraga – poštansko sanduče</span><span class="sxs-lookup"><span data-stu-id="cfdc6-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="cfdc6-114">Za Poštanske sandučiće na čekanju, administratori moraju da uklone čekanje pre nego što mogu da izbrišu stavke iz fascikle "stavke koje se mogu spasti".</span><span class="sxs-lookup"><span data-stu-id="cfdc6-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="cfdc6-115">Više informacija potražite u članku [Brisanje stavki u fascikli "pristupačnije stavke" sa poštanskim sandučićima zasnovanim na oblaku](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="cfdc6-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="cfdc6-116">Da bi se sprečilo da fascikla sa ispravnošću može da postane puna, administratori mogu da povećaju ograničenje skladišta stavki "Oporadne stavke" za Poštanske sandučiće na čekanju i podesite smernice za zadržavanje poštanskog sandučeta koje pomeraju stavke iz fascikle "Oporadne stavke" u skladište primaoca.</span><span class="sxs-lookup"><span data-stu-id="cfdc6-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="cfdc6-117">Pogledajte članak povećanje kvote pristupačnih [stavki za Poštanske sandučiće na čekanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="cfdc6-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
