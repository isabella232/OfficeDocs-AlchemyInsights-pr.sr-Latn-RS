---
title: Premeštanje e-poruka u poštansko sanduče arhive
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799794"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="bc862-102">Premeštanje e-pošte u poštansko sanduče arhive</span><span class="sxs-lookup"><span data-stu-id="bc862-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="bc862-103">Ako želite da uradite automatizovane provere za postavke navedene ispod, kliknite na dugme nazad <, na vrhu ove stranice, a zatim unesite e-adresu korisnika koji ima problema sa premeštanjem e-pošte u poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="bc862-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="bc862-104">Potvrdite da je **arhivirane poštansko sanduče** omogućeno.</span><span class="sxs-lookup"><span data-stu-id="bc862-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="bc862-105">Ako nije, koristite korake u [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da biste omogućili Arhiviraj poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="bc862-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="bc862-106">Da biste automatski arhivirati poruke u poštansko sanduče arhive, oznaka za zadržavanje sa akcijom " **Premesti u arhivu** " mora biti postavljena tako da se **automatski primeni na celu nalepnicu sa poštanskim sandučetom (podrazumevana vrednost)**.</span><span class="sxs-lookup"><span data-stu-id="bc862-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="bc862-107">Koristite ove korake da biste kreirali oznaku: [Podrazumevana oznaka arhivira](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="bc862-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="bc862-108">Zatim dodajte oznaku **arhive** u smernice za zadržavanje.</span><span class="sxs-lookup"><span data-stu-id="bc862-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="bc862-109">U Exchange centru administracije odaberite smernice za **zadržavanje** > dodajte **Premeštanje u oznaku arhiviranja** na smernice > **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="bc862-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="bc862-110">Sada [dodelite smernice za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) za poštansko sanduče određenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="bc862-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="bc862-111">Iste smernice će se primeniti i na **primarno** i u poštansko sanduče **arhive** .</span><span class="sxs-lookup"><span data-stu-id="bc862-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="bc862-112">Možda će biti neophodno da se korisnik kontrolisane fascikle (MFA) pokreće i primenjuje nove postavke na poštansko sanduče korisnika.</span><span class="sxs-lookup"><span data-stu-id="bc862-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="bc862-113">Pokrenite sledeću komandu dok ste [povezani sa EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnika kontrolisane fascikle za određeno poštansko sanduče:</span><span class="sxs-lookup"><span data-stu-id="bc862-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="bc862-114">Start-Managedderderik-identitet <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="bc862-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="bc862-115">Više informacija o podešavanju smernica za arhiviranje potražite u članku [Podešavanje smernica za arhiviranje i brisanje za Poštanske sandučiće](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="bc862-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  