---
title: 126 preuzimanje poštanskog sandučeta ne može da se pronađe greška u programu OWA?
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
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706764"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="e980d-102">Preuzimanje greške poštanskog sandučeta u programu Outlook na vebu?</span><span class="sxs-lookup"><span data-stu-id="e980d-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="e980d-103">Ako koristite Outlook na vebu i dobijate **poštansko sanduče ne može da se pronađe za** grešku, nalog koji ste koristili za povezivanje sa programom Outlook na vebu nema Exchange online licencu i zato nije povezan nijedan poštansko sanduče sa nalogom.</span><span class="sxs-lookup"><span data-stu-id="e980d-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="e980d-104">Administrator može da dodeli licencu nalogu tako što će pratiti ove korake:</span><span class="sxs-lookup"><span data-stu-id="e980d-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="e980d-105">Otvorite [Microsoft 365 centar administracije](https://portal.office.com/adminportal/home#/homepage) i idite na **aktivne korisnike** u odeljku **Korisnici** i izaberite korisnika koji vidi grešku.</span><span class="sxs-lookup"><span data-stu-id="e980d-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="e980d-106">Na stranici korisnika koja se otvara idite na odeljak **licence i aplikacije** , izaberite odgovarajuću vrednost **lokacije** i dodelite licencu koja sadrži Exchange Online (proširite licencu da biste videli detalje).</span><span class="sxs-lookup"><span data-stu-id="e980d-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="e980d-107">Kada završite, kliknite na dugme **Sačuvaj promene**.</span><span class="sxs-lookup"><span data-stu-id="e980d-107">When you're finished, click **Save changes**.</span></span>
