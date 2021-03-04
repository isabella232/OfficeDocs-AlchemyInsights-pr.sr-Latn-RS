---
title: Potvrdite izbor u polju za potvrdu prosleđivanje adresa na poštanski sandučićima
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427711"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="015ba-102">Potvrdite izbor u polju za potvrdu prosleđivanje adresa na poštanski sandučićima</span><span class="sxs-lookup"><span data-stu-id="015ba-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="015ba-103">Ponekad hakera unapred prosleđuje e-poruke korisnicima, tako da ćemo prvo da proverimo da li postoje adrese i pravila za poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="015ba-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="015ba-104">Zatim ćemo provjeriti evidentira nadgledanja.</span><span class="sxs-lookup"><span data-stu-id="015ba-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="015ba-105">Evo kako da potvrdite izbor u polju za prosleđivanje:</span><span class="sxs-lookup"><span data-stu-id="015ba-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="015ba-106">Izbor **korisnika**  >  **aktivnih korisnika**.</span><span class="sxs-lookup"><span data-stu-id="015ba-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="015ba-107">Izaberite korisnika čiji nalog je kompromitovan.</span><span class="sxs-lookup"><span data-stu-id="015ba-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="015ba-108">U poruci koja se pojavi razvijte **postavke pošte**, a zatim izaberite stavku **Uredi** za **Prosleđivanje e-pošte**.</span><span class="sxs-lookup"><span data-stu-id="015ba-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="015ba-109">Uklonite sve prosleđivanje adresa koje ne prepoznate.</span><span class="sxs-lookup"><span data-stu-id="015ba-109">Remove any forwarding addresses you don't recognize.</span></span>