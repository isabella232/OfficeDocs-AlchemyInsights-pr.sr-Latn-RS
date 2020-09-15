---
title: Nedostaju e-poruke u karantinu
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673728"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="ffbff-102">Nedostaju e-poruke u karantinu "</span><span class="sxs-lookup"><span data-stu-id="ffbff-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="ffbff-103">Administratori mogu da [prikažu, oslobode ili izbrišu ove poruke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ffbff-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="ffbff-104">Da biste otvorili bezbednosni & centar za usaglašenost, idite na [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="ffbff-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="ffbff-105">Da biste otvorili stranicu karantina direktno, idite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="ffbff-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="ffbff-106">Možete da pretražujete po sledećim vrednostima:</span><span class="sxs-lookup"><span data-stu-id="ffbff-106">You can search by the following values:</span></span>  

- <span data-ttu-id="ffbff-107">**ID poruke**: globalni Jedinstveni identifikator poruke.</span><span class="sxs-lookup"><span data-stu-id="ffbff-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="ffbff-108">Ako na listi izaberete poruku, vrednost ID-a  **poruke**  se pojavljuje u oknu "razmeni za  **detalje**  " koji se pojavljuje.</span><span class="sxs-lookup"><span data-stu-id="ffbff-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="ffbff-109">Administratori mogu da koriste [praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) da bi pronašli poruke i ODGOVARAJUĆE vrednosti ID-a poruka.</span><span class="sxs-lookup"><span data-stu-id="ffbff-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="ffbff-110">**Adresa pošiljaoca**: e-adresa jednog pošiljaoca.</span><span class="sxs-lookup"><span data-stu-id="ffbff-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="ffbff-111">**Adresa e-pošte primaoca**: e-adresa za primaoca.</span><span class="sxs-lookup"><span data-stu-id="ffbff-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="ffbff-112">**Tema**: koristite celu temu poruke.</span><span class="sxs-lookup"><span data-stu-id="ffbff-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="ffbff-113">Pretraga ne razlikuje mala i velika slova.</span><span class="sxs-lookup"><span data-stu-id="ffbff-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="ffbff-114">Kada unesete kriterijume pretrage, kliknite na dugme ![ Osveži ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **osvežavanje** dugmeta da biste filtrirali rezultate.  </span><span class="sxs-lookup"><span data-stu-id="ffbff-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="ffbff-115">Cmdlet koji koristite za prikazivanje poruka i datoteka u karantinu su:</span><span class="sxs-lookup"><span data-stu-id="ffbff-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="ffbff-116">Brisanje iz karantina poruka</span><span class="sxs-lookup"><span data-stu-id="ffbff-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="ffbff-117">Izvoz-poruka u karantinu</span><span class="sxs-lookup"><span data-stu-id="ffbff-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="ffbff-118">Poruka u karantinu</span><span class="sxs-lookup"><span data-stu-id="ffbff-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="ffbff-119">[Pregled u karantinu](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Imajte na umu da je ova cmdlet poruka samo za poruke, a ne za datoteke malver sa ATP-a za SharePoint online, OneDrive for Business ili timove.</span><span class="sxs-lookup"><span data-stu-id="ffbff-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="ffbff-120">Izdanje-karantin poruka</span><span class="sxs-lookup"><span data-stu-id="ffbff-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)