---
title: 126 Nije moguće pronaći grešku Pribavljanje poštanskog sandučeta u programu OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426676"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="b6e11-102">Dobijate grešku "Nije pronađeno poštansko sanduče" u programu Outlook na vebu?</span><span class="sxs-lookup"><span data-stu-id="b6e11-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="b6e11-103">Ako koristite Outlook na vebu i  ne možete da dobijete grešku u Poštanskom sandučetu, nalog koji ste koristili za povezivanje sa programom Outlook na vebu nema Exchange Online licencu i zbog toga nijedno poštansko sanduče nije povezano sa nalogom.</span><span class="sxs-lookup"><span data-stu-id="b6e11-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="b6e11-104">Vaš administart može da dodeli licencu vašem nalogu tako što će pratiti ove korake:</span><span class="sxs-lookup"><span data-stu-id="b6e11-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="b6e11-105">Otvorite [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) centar za administaciju i idite na stavku Aktivni korisnici u odeljku Korisnici i izaberite korisnika koji vidite grešku.  </span><span class="sxs-lookup"><span data-stu-id="b6e11-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="b6e11-106">Na stranici korisnika koja se  otvori, idite na odeljak Licence i aplikacije, izaberite odgovarajuću vrednost lokacije i dodelite licencu koja sadrži Exchange Online (razvijte licencu da biste videli detalje o njoj). </span><span class="sxs-lookup"><span data-stu-id="b6e11-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="b6e11-107">Kada završite, kliknite na dugme **Sačuvaj promene.**</span><span class="sxs-lookup"><span data-stu-id="b6e11-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="b6e11-108">U nekim slučajevima, ako je licenca već dodeljena korisničkom nalogu, uklanjanje i ponovna dodela licence pomaže u rešavanju problema i ispravno je obezbeđena u sistemu:</span><span class="sxs-lookup"><span data-stu-id="b6e11-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="b6e11-109">Proverite da li su vaše M365 Exchange Online (i druge, ako ih imate) aktuelne i da nisu nedavno istekle.</span><span class="sxs-lookup"><span data-stu-id="b6e11-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="b6e11-110">Kada se uverite da vam pretplata nije istekla i da je dodeljena važeća licenca korisničkom nalogu, do obezbeđivanje licence može da protekne i do 24 časa, tako da ćete možda morati da sačekate da se problem reši.</span><span class="sxs-lookup"><span data-stu-id="b6e11-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="b6e11-111">Dodatne informacije potražite u [članku Dodeljivanje licenci i upravljanje im.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="b6e11-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>