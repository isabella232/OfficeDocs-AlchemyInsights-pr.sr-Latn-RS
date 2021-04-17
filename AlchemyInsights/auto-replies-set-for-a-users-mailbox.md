---
title: Postavljanje automatskih odgovora za poštansko sanduče
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820948"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="c7102-102">Postavljanje automatskih odgovora za poštansko sanduče korisnika</span><span class="sxs-lookup"><span data-stu-id="c7102-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="c7102-103">**Metod 1**</span><span class="sxs-lookup"><span data-stu-id="c7102-103">**Method 1**</span></span>

1. <span data-ttu-id="c7102-104">Prijavljivanje u Microsoft 365 portal.</span><span class="sxs-lookup"><span data-stu-id="c7102-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="c7102-105">Idite na stavku **Korisnici > Aktivni korisnici** (ili **Grupe > Deljeni poštanski sandučići** ako ste postavili ovo na deljeno poštansko sanduče).</span><span class="sxs-lookup"><span data-stu-id="c7102-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="c7102-106">Izaberite korisnika koji ima Microsoft Exchange poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="c7102-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="c7102-107">U dodatnom meniju nadesno idite na **Postavke pošte > Automatski odgovori**(ako je u pitanju deljeno poštansko sanduče, samo kliknite **Automatski odgovori** u dodatnom meniju).</span><span class="sxs-lookup"><span data-stu-id="c7102-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="c7102-108">**Metod 2**</span><span class="sxs-lookup"><span data-stu-id="c7102-108">**Method 2**</span></span>

1. <span data-ttu-id="c7102-109">Prijavite se na Microsoft 365 portal za administraciju pomoću akreditiva administratora.</span><span class="sxs-lookup"><span data-stu-id="c7102-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="c7102-110">Proširite **Centre za administraciju**, a zatim kliknite na stavku **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c7102-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="c7102-111">Kliknite na sliku u gornjem desnom uglu, kliknite na stavku **Još jedan korisnik**, a zatim izaberite korisničko poštansko sanduče koje želite da promenite.</span><span class="sxs-lookup"><span data-stu-id="c7102-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="c7102-112">Na levoj strani izaberite stavku **Opcije**, kliknite na stavku **Organizovanje e-pošte**, a zatim kliknite na dugme **Automatski odgovori.**</span><span class="sxs-lookup"><span data-stu-id="c7102-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="c7102-113">**Metod 3**</span><span class="sxs-lookup"><span data-stu-id="c7102-113">**Method 3**</span></span>

<span data-ttu-id="c7102-114">Pokrenite sledeće cmdlet komandu u usluzi Exchange Online Windows PowerShell:</span><span class="sxs-lookup"><span data-stu-id="c7102-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="c7102-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="c7102-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="c7102-116">Više informacija o ovoj cmdlet komandi potražite u članku [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="c7102-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
