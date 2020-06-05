---
title: Nedostajuće e-poruke u karantinu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569558"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="76852-102">Nedostaju e-poruke u karantinu "</span><span class="sxs-lookup"><span data-stu-id="76852-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="76852-103">Administratori mogu da [prikažu, puste ili izbrišu ove poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="76852-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="76852-104">Da biste otvorili bezbednosni & centar za usaglašavanje, idite na lokaciju [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="76852-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="76852-105">Idite na stranicu "karantin" da biste je otvorili direktno [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="76852-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="76852-106">Možete pretraživati po sledećim vrednostima:</span><span class="sxs-lookup"><span data-stu-id="76852-106">You can search by the following values:</span></span>  

- <span data-ttu-id="76852-107">**ID poruke**: univerzalni jedinstveni identifikator poruke.</span><span class="sxs-lookup"><span data-stu-id="76852-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="76852-108">Ako izaberete poruku na listi, vrednost **ID poruke** će se pojaviti u oknu " **Detalji** " koji se pojavljuje.</span><span class="sxs-lookup"><span data-stu-id="76852-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="76852-109">Administratori mogu da koriste [praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) da bi pronašli poruke i njihove odgovarajuće ID vrednosti poruka.</span><span class="sxs-lookup"><span data-stu-id="76852-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="76852-110">**E-adresa pošiljaoca**: adresa e-pošte jednog pošiljaoca.</span><span class="sxs-lookup"><span data-stu-id="76852-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="76852-111">**E-adresa primaoca**: e-adresa jednog primaoca.</span><span class="sxs-lookup"><span data-stu-id="76852-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="76852-112">**Tema**: koristite čitavu temu poruke.</span><span class="sxs-lookup"><span data-stu-id="76852-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="76852-113">Pretraga ne razlikuje mala i velika slova.</span><span class="sxs-lookup"><span data-stu-id="76852-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="76852-114">Nakon što ste uneli kriterijume pretrage, kliknite na ![ dugme "Osveži" ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži** da biste filtrirali rezultate.  </span><span class="sxs-lookup"><span data-stu-id="76852-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="76852-115">Cmdlet omogućava korišćenje za prikaz i upravljanje porukama i datotekama u karantinu:</span><span class="sxs-lookup"><span data-stu-id="76852-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="76852-116">Izbriši-Neu karantin</span><span class="sxs-lookup"><span data-stu-id="76852-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="76852-117">EXPORT-u karantin</span><span class="sxs-lookup"><span data-stu-id="76852-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="76852-118">-U Karantinda</span><span class="sxs-lookup"><span data-stu-id="76852-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="76852-119">[Preview-Ukarantu u karantin](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ova cmdonly samo za poruke, a ne za datoteke MALVERA iz ATP-a za SharePoint online, OneDrive za poslovanje ili timove.</span><span class="sxs-lookup"><span data-stu-id="76852-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="76852-120">Pusti to</span><span class="sxs-lookup"><span data-stu-id="76852-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)