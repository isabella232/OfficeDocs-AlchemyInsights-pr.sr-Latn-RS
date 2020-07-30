---
title: Premeštanje e-poruka u poštansko sanduče arhive
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522785"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="c7f0e-102">Premeštanje e-poruke u poštansko sanduče arhive</span><span class="sxs-lookup"><span data-stu-id="c7f0e-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="c7f0e-103">Ako želite da pokrećemo automatske provere za gore pomenute postavke, kliknite na dugme "nazad" <--na vrhu ove stranice, a zatim unesite e-adresu korisnika koji ima problema prilikom premeštanja e-pošte u poštansko sanduče arhive.</span><span class="sxs-lookup"><span data-stu-id="c7f0e-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="c7f0e-104">Potvrdite da je **poštansko sanduče arhive** omogućeno.</span><span class="sxs-lookup"><span data-stu-id="c7f0e-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="c7f0e-105">Ako ne, koristite korake iz [ovog članka](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da biste omogućili poštansko sanduče arhive.</span><span class="sxs-lookup"><span data-stu-id="c7f0e-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="c7f0e-106">Da bi se poruke automatski arhivirali u poštansko sanduče arhive, oznaka za zadržavanje sa radnjom " **Premesti u arhivu** " mora biti podešena tako da se **automatski primenjuje u celokupnu oznaku "poštansko sanduče" (podrazumevana)**.</span><span class="sxs-lookup"><span data-stu-id="c7f0e-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="c7f0e-107">Koristite korake ovde da biste kreirali oznaku: [Arhiviraj podrazumevanu oznaku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="c7f0e-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="c7f0e-108">Zatim dodajte oznaku **arhive** u smernice za zadržavanje.</span><span class="sxs-lookup"><span data-stu-id="c7f0e-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="c7f0e-109">U Exchange admin Center izaberite smernice za **zadržavanje** > dodajte stavku " **Premesti u** " u smernicu > " **Sačuvaj**".</span><span class="sxs-lookup"><span data-stu-id="c7f0e-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="c7f0e-110">Sada [dodelite smernice za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) u poštansko sanduče određenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="c7f0e-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="c7f0e-111">Ista smernica će se primeniti i na **primarnu** i u poštansko sanduče **arhive** .</span><span class="sxs-lookup"><span data-stu-id="c7f0e-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="c7f0e-112">Možda će biti neophodno da naterate pomoćnika za upravljane fascikle (MFA) da pokrećete i primenite nove postavke na korisnikovo poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="c7f0e-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="c7f0e-113">Pokrenite sledeću komandu dok [ste povezani sa EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnika za kontrolisanu fasciklu za određeno poštansko sanduče:</span><span class="sxs-lookup"><span data-stu-id="c7f0e-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="c7f0e-114">Start-ManagedFolderAssistant-identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="c7f0e-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="c7f0e-115">Više informacija o podešavanju smernica arhive potražite [u članku Podešavanje smernica za arhiviranje i brisanje za Poštanske sandučiće](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="c7f0e-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  