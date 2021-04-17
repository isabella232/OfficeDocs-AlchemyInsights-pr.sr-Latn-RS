---
title: E-poruke koje nedostaju u karantinu
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
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831748"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="c282a-102">E-poruke koje nedostaju u karantinu"</span><span class="sxs-lookup"><span data-stu-id="c282a-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="c282a-103">Administratori mogu da [pregledaju, izbrišu ili izbrišu ove poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="c282a-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="c282a-104">Da biste otvorili centar & za usaglašenost, idite na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="c282a-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="c282a-105">Da biste direktno otvorili stranicu Karantin, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="c282a-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="c282a-106">Možete pretražiti po sledećim vrednostima:</span><span class="sxs-lookup"><span data-stu-id="c282a-106">You can search by the following values:</span></span>  

- <span data-ttu-id="c282a-107">**ID poruke:** Globalni jedinstveni identifikator poruke.</span><span class="sxs-lookup"><span data-stu-id="c282a-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="c282a-108">Ako izaberete poruku sa liste, vrednost  **ID-a**  poruke se pojavljuje u  **oknu**  ileta Detalji koje se pojavljuje.</span><span class="sxs-lookup"><span data-stu-id="c282a-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="c282a-109">Da bi pronašli poruke i njihove odgovarajuće [vrednosti](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) ID-a poruke, a mogu da koriste i funkciju "Praćenje poruka".</span><span class="sxs-lookup"><span data-stu-id="c282a-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="c282a-110">**Adresa e-pošte** pošiljaoca: adresa e-pošte jednog pošiljaoca.</span><span class="sxs-lookup"><span data-stu-id="c282a-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="c282a-111">**Adresa e-pošte** primaoca: E-adresa jednog primaoca.</span><span class="sxs-lookup"><span data-stu-id="c282a-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="c282a-112">**Tema:** Koristite celu temu poruke.</span><span class="sxs-lookup"><span data-stu-id="c282a-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="c282a-113">Pretraga ne osetljiva na velika i velika slova.</span><span class="sxs-lookup"><span data-stu-id="c282a-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="c282a-114">Kada unesete kriterijume za pretragu, kliknite na dugme ![ Osveži dugme ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži da** biste filtrirali rezultate.  </span><span class="sxs-lookup"><span data-stu-id="c282a-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="c282a-115">Cmdlet grupe koje koristite za prikaz poruka i datoteka i upravljanje datotekama u karantinu su:</span><span class="sxs-lookup"><span data-stu-id="c282a-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="c282a-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c282a-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="c282a-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c282a-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="c282a-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c282a-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="c282a-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Imajte uvid u to da je ova cmdlet datoteka samo za poruke, a ne za malver datoteke iz ATP sistema za SharePoint Online, OneDrive for Business ili Teams.</span><span class="sxs-lookup"><span data-stu-id="c282a-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="c282a-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="c282a-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)