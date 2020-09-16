---
title: Smernice za zadržavanje u Exchange centru administracije ne funkcionišu
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740524"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="1f4df-102">Smernice za zadržavanje u Exchange centru administracije</span><span class="sxs-lookup"><span data-stu-id="1f4df-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="1f4df-103">Ako želite da uradite automatizovane provere za postavke navedene ispod, kliknite na dugme nazad <, na vrhu ove stranice, a zatim unesite e-adresu korisnika koji ima problema sa smernicama za zadržavanje.</span><span class="sxs-lookup"><span data-stu-id="1f4df-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="1f4df-104">**Problem:** Nove kreirane ili ažurirane smernice za zadržavanje u Exchange centru administracije se ne primenjuju na Poštanske sandučiće ili stavke se ne pomeraju u poštansko sanduče arhiva ili izbrisane.</span><span class="sxs-lookup"><span data-stu-id="1f4df-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="1f4df-105">**Osnovni uzroci:**</span><span class="sxs-lookup"><span data-stu-id="1f4df-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="1f4df-106">To je možda zato što **Pomoćnik kontrolisane fascikle** nije obradio poštansko sanduče korisnika.</span><span class="sxs-lookup"><span data-stu-id="1f4df-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="1f4df-107">Pomoćnik kontrolisane fascikle pokušava da obradi svako poštansko sanduče u organizaciji zasnovanoj na oblaku na svakih sedam dana.</span><span class="sxs-lookup"><span data-stu-id="1f4df-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="1f4df-108">Ako promenite oznaku za zadržavanje ili primenite različitu polisu za zadržavanje na poštansko sanduče, možete da sačekate dok Kontrolisana fascikla ne obradi poštansko sanduče ili možete da pokrenete program "Start-Managederderderik" koji će obraditi određeno poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="1f4df-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="1f4df-109">Pokretanje ovog cmdlet funkcije je korisno za testiranje ili rešavanje problema sa postavkama oznake za zadržavanje ili označavanje.</span><span class="sxs-lookup"><span data-stu-id="1f4df-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="1f4df-110">Više informacija potražite u odeljku ["Pomoćnik za upravljanje fasciklama](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)".</span><span class="sxs-lookup"><span data-stu-id="1f4df-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="1f4df-111">**Rešenje:** Pokrenite sledeću komandu da biste pokrenuli pomoćnika kontrolisane fascikle za određeno poštansko sanduče:</span><span class="sxs-lookup"><span data-stu-id="1f4df-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="1f4df-112">To se može desiti i ako je **zadržavanje** **omogućeno** na poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="1f4df-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="1f4df-113">Ako je poštansko sanduče postavljeno na čekanje, smernice za zadržavanje na poštanskom sandučetu neće biti obrađene tokom tog vremena.</span><span class="sxs-lookup"><span data-stu-id="1f4df-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="1f4df-114">Za više Informatika na stranici zadržavanje pogledajte članak: [čekanje zadržavanja poštanskog sandučeta](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="1f4df-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="1f4df-115">**Raspada**</span><span class="sxs-lookup"><span data-stu-id="1f4df-115">**Solution:**</span></span>
    
  - <span data-ttu-id="1f4df-116">Potvrdite status postavke zadržavanja na određenom poštanskom sandučetu u [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="1f4df-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="1f4df-117">Uradite sledeće komande da biste **onemogućili** čekanje na određeno poštansko sanduče:</span><span class="sxs-lookup"><span data-stu-id="1f4df-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="1f4df-118">Sada ponovo vodite pomoćnika kontrolisanog fascikle:</span><span class="sxs-lookup"><span data-stu-id="1f4df-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="1f4df-119">**Napomena:** Ako je poštansko sanduče manje od 10 MB, pomoćnik kontrolisane fascikle neće automatski obraditi poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="1f4df-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="1f4df-120">Više informacija o smernicama za zadržavanje u Exchange centru administracije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="1f4df-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="1f4df-121">Oznake za zadržavanje i smernice za zadržavanje</span><span class="sxs-lookup"><span data-stu-id="1f4df-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="1f4df-122">Primenjivanje smernica za zadržavanje na Poštanske sandučiće</span><span class="sxs-lookup"><span data-stu-id="1f4df-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="1f4df-123">Dodavanje ili uklanjanje oznaka za zadržavanje</span><span class="sxs-lookup"><span data-stu-id="1f4df-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="1f4df-124">Kako da identifikujete tip čekanja postavljeno na poštansko sanduče</span><span class="sxs-lookup"><span data-stu-id="1f4df-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
