---
title: Smernice za zadržavanje u sistemu Exchange admin Center ne rade
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522821"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="742b0-102">Smernice za zadržavanje u programu Exchange admin Center</span><span class="sxs-lookup"><span data-stu-id="742b0-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="742b0-103">Ako želite da pokrećemo automatske provere za gore pomenute postavke, kliknite na dugme "nazad" <--na vrhu ove stranice, a zatim unesite e-adresu korisnika koji ima problema sa smernicama za zadržavanje.</span><span class="sxs-lookup"><span data-stu-id="742b0-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="742b0-104">**Problem:** Nove ili ažurirane smernice za zadržavanje u Exchange admin Center ne primenjuju se na Poštanske sandučiće ili stavke nisu premeštene u poštansko sanduče arhive ili su izbrisane.</span><span class="sxs-lookup"><span data-stu-id="742b0-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="742b0-105">**Osnovni uzroci:**</span><span class="sxs-lookup"><span data-stu-id="742b0-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="742b0-106">Ovo je možda zbog toga što **Pomoćnik kontrolisane fascikle** nije obradio korisnikovo poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="742b0-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="742b0-107">Pomoćnik kontrolisane fascikle pokušava da obradi svako poštansko sanduče u organizaciji zasnovanom na informatičkom oblaku jednom u sedam dana.</span><span class="sxs-lookup"><span data-stu-id="742b0-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="742b0-108">Ako promenite oznaku za zadržavanje ili primenite drugačije smernice za zadržavanje u poštansko sanduče, možete sačekati da Kontrolisana fascikla pomogne u obradi poštanskog sandučeta, ili možete da pokrenete Start-ManagedFolderAssistant cmdda biste pokrenuli pomoćnik za kontrolisane fascikle da biste obradili određeno poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="742b0-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="742b0-109">Pokretanje ove cmdmo komande je korisno za testiranje ili rešavanje problema sa postavkama za zadržavanje ili za zadržavanje oznaka zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="742b0-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="742b0-110">Za više informacija posjetite [pokrenite pomoćnika za Upravljnju fasciklu](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="742b0-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="742b0-111">**Rešenje:** Pokrenite sledeću komandu da biste pokrenuli pomoćnik za kontrolisane fascikle za određeno poštansko sanduče:</span><span class="sxs-lookup"><span data-stu-id="742b0-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="742b0-112">Do ovoga može doći i ako je u poštanskom sandučetu **omogućen** **retencionent** .</span><span class="sxs-lookup"><span data-stu-id="742b0-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="742b0-113">Ako je poštansko sanduče postavljeno na Retencioniku, smernice za zadržavanje u poštanskom sandučetu neće biti obrađene u tom trenutku.</span><span class="sxs-lookup"><span data-stu-id="742b0-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="742b0-114">Za dodatne informacije o postavci Retentionzadrške pogledajte: [zadržavanje poštanskog sandučeta](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="742b0-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="742b0-115">**Rešenje:**</span><span class="sxs-lookup"><span data-stu-id="742b0-115">**Solution:**</span></span>
    
  - <span data-ttu-id="742b0-116">Proverite status postavke Retentiondržanja na određenom poštanskom sandučetu u [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="742b0-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="742b0-117">Pokrenite sledeću komandu da biste **onemogućili** retentioniste na određenom poštanskom sandučetu:</span><span class="sxs-lookup"><span data-stu-id="742b0-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="742b0-118">Sada ponovo pokrenite pomoćnika za upravljane fascikle:</span><span class="sxs-lookup"><span data-stu-id="742b0-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="742b0-119">**Napomena:** Ako je poštansko sanduče manje od 10 MB, pomoćnik za Upravljnu fasciklu neće automatski obraditi poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="742b0-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="742b0-120">Više informacija o smernicama za zadržavanje u Exchange admin Center potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="742b0-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="742b0-121">Zadržavanjem oznaka i smernica zadržavanja</span><span class="sxs-lookup"><span data-stu-id="742b0-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="742b0-122">Primenjivanje smernica za zadržavanje u Poštanske sandučiće</span><span class="sxs-lookup"><span data-stu-id="742b0-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="742b0-123">Dodavanje ili uklanjanje oznaka za zadržavanje</span><span class="sxs-lookup"><span data-stu-id="742b0-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="742b0-124">Identifikovanje tipa zadrška koji se postavlja u poštansko sanduče</span><span class="sxs-lookup"><span data-stu-id="742b0-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
