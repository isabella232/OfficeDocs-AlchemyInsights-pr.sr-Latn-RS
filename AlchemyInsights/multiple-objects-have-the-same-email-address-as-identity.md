---
title: Više objekata ima istu e-adresu kao identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439712"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="cc36e-102">Više objekata ima istu e-adresu kao identitet</span><span class="sxs-lookup"><span data-stu-id="cc36e-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="cc36e-103">**Više objekata**</span><span class="sxs-lookup"><span data-stu-id="cc36e-103">**Multiple objects**</span></span>

<span data-ttu-id="cc36e-104">Jedan od uobičajenih razloga ove greške nije u mogućnosti da usmeri zahtev za Outlook Web Access na odgovarajući način u prisustvu više objekata koji imaju istu e-adresu kao identitet.</span><span class="sxs-lookup"><span data-stu-id="cc36e-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="cc36e-105">Da biste pronašli ove objekte, pokrenite sledeće komande:</span><span class="sxs-lookup"><span data-stu-id="cc36e-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="cc36e-106">· Nabavi primaocu<email address></span><span class="sxs-lookup"><span data-stu-id="cc36e-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="cc36e-107">· Dobijanje korisnika<email address></span><span class="sxs-lookup"><span data-stu-id="cc36e-107">· Get-User <email address></span></span>

<span data-ttu-id="cc36e-108">· Get-korisnik <email address> -softdeleteduser</span><span class="sxs-lookup"><span data-stu-id="cc36e-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="cc36e-109">· Preuzimanje-kontakt<email address></span><span class="sxs-lookup"><span data-stu-id="cc36e-109">· Get-Contact <email address></span></span>

<span data-ttu-id="cc36e-110">· Get-poštansko sanduče <email address> -publikfascikla</span><span class="sxs-lookup"><span data-stu-id="cc36e-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="cc36e-111">· Preuzimanje-poštansko sanduče <email address> -includesoftdeletedpoštansko sanduče</span><span class="sxs-lookup"><span data-stu-id="cc36e-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="cc36e-112">· Preuzimanje-poštansko sanduče <email address> -inactivemailboxonly</span><span class="sxs-lookup"><span data-stu-id="cc36e-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="cc36e-113">Da biste rešili ovaj problem, uklonite više objekata sa istim identitetom e-pošte i uverite se da postoji jedan objekat sa određenim identitetom e-pošte i da je njegov tip primaoca Userpoštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="cc36e-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="cc36e-114">**Ista adresa se koristi za poslovne i potrošačke Poštanske sandučiće**</span><span class="sxs-lookup"><span data-stu-id="cc36e-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="cc36e-115">Drugi uzrok je kada se ista adresa koristi za poslovne i potrošačke Poštanske sandučiće.</span><span class="sxs-lookup"><span data-stu-id="cc36e-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="cc36e-116">U ovom slučaju, korisnik mora da promeni primarni pseudonim za potrošače dok CAFFE ne podržava ovaj scenario.</span><span class="sxs-lookup"><span data-stu-id="cc36e-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="cc36e-117">Ovo je stalna greška koja ne nestane bez intervencije.</span><span class="sxs-lookup"><span data-stu-id="cc36e-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="cc36e-118">Više informacija potražite u članku [Promena e-adrese ili broja telefona za Microsoft nalog](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="cc36e-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>