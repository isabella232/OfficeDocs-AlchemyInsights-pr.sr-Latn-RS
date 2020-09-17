---
title: Omogućavanje arhiviranja arhive
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811720"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="a1cdc-102">Omogućavanje arhiviranja arhive</span><span class="sxs-lookup"><span data-stu-id="a1cdc-102">Enable an archive mailbox</span></span>

<span data-ttu-id="a1cdc-103">Ako želite da izvršit automatsku proveru da biste obezbedili da arhivirane poštansko sanduče može da se podesi, kliknite na dugme nazad <, na vrhu ove stranice, a zatim unesite e-adresu naloga.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="a1cdc-104">Arhiviranje poštanskih sandučića u sistemu Microsoft 365 (koje se takođe naziva i arhivske *arhive* ili *arhiv arhiva*) pružaju korisnicima dodatni prostor za skladištenje e-pošte.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="a1cdc-105">Korisnici mogu da pomeraju ili kopiraju stavke u poštansko sanduče arhive, a administratori mogu da kreiraju smernice za arhiviranje koje automatski pomeraju stavke da bi arhiviraju Poštanske sandučiće.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="a1cdc-106">Evo kako da kreirate poštansko sanduče arhive:</span><span class="sxs-lookup"><span data-stu-id="a1cdc-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="a1cdc-107">Idite na [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="a1cdc-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="a1cdc-108">Prijavite se u Microsoft 365 pomoću administratorskog naloga.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="a1cdc-109">U levom oknu centra za bezbednost &amp; usaglašenosti izaberite arhivu **upravljanja informacijama** \> **Archive**.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="a1cdc-110">Izaberite korisnika čije arhiviranje poštanskog sandučeta želite da omogućite.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="a1cdc-111">U oknu sa detaljima sa desne strane izaberite stavku **Omogućavanje** , a zatim kliknite na dugme **da** u poruci upozorenja da biste omogućili Arhiviraj poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="a1cdc-112">Arhiviranjem arhivskih poštanskih sandučića takođe možete da razradite tako što ćete izabrati više korisnika (koristite **SHIFT** ili **Ctrl** ), a zatim kliknuti na dugme **Omogućavanje** u oknu sa detaljima.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="a1cdc-113">Deljeni poštanski sandučići</span><span class="sxs-lookup"><span data-stu-id="a1cdc-113">Shared mailboxes</span></span>

<span data-ttu-id="a1cdc-114">Da biste omogućili arhivu za Deljeno poštansko sanduče, potrebna je licenca Exchange online plan 2 ili Exchange online plan 1 licence sa licencom za arhiviranje Exchange online.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="a1cdc-115">Da biste omogućili arhiviranje deljenog poštanskog sandučeta:</span><span class="sxs-lookup"><span data-stu-id="a1cdc-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="a1cdc-116">Idite u [Exchange centar administracije](https://outlook.office365.com/ecp) i prijavite se pomoću administratorskog naloga.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="a1cdc-117">Idite na **Deljeni primalac primalaca**  >  **Shared**.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="a1cdc-118">Izaberite Deljeno poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="a1cdc-119">U oknu sa detaljima sa desne strane, u okviru **arhiv**, kliknite na dugme **Omogućavanje**, a zatim kliknite na dugme **da** da biste omogućili Arhiviraj poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="a1cdc-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="a1cdc-120">Za više informacija pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="a1cdc-120">For more information, see:</span></span>
  
- [<span data-ttu-id="a1cdc-121">Omogućavanje arhiviranja poštanskih sandučića</span><span class="sxs-lookup"><span data-stu-id="a1cdc-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="a1cdc-122">Podešavanje smernica za arhiviranje i brisanje</span><span class="sxs-lookup"><span data-stu-id="a1cdc-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
