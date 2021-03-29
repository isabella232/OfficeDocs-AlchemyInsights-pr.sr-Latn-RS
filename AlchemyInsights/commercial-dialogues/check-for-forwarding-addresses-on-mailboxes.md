---
title: Proverite da li ima adresa za prosleđivanje u poštanskim sandučićima
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403325"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="30b01-102">Proverite da li ima adresa za prosleđivanje u poštanskim sandučićima</span><span class="sxs-lookup"><span data-stu-id="30b01-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="30b01-103">Ponekad hakeri prosleđuju e-poruke korisnika na sebe, pa ćemo prvo proveriti da li postoje adrese za prosleđivanje i pravila u poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="30b01-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="30b01-104">Zatim ćemo proveriti evidencije nadzora.</span><span class="sxs-lookup"><span data-stu-id="30b01-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="30b01-105">Evo kako da proverite da li ima adresa za prosleđivanje:</span><span class="sxs-lookup"><span data-stu-id="30b01-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="30b01-106">Izaberite **stavku Korisnici**  >  **aktivni korisnici**.</span><span class="sxs-lookup"><span data-stu-id="30b01-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="30b01-107">Izaberite korisnika čiji nalog je ugrožen.</span><span class="sxs-lookup"><span data-stu-id="30b01-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="30b01-108">U iletu koji se pojavi razvijte stavku **Postavke** pošte , a zatim izaberite stavku Uredi **za** **prosleđivanje e-pošte.**</span><span class="sxs-lookup"><span data-stu-id="30b01-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="30b01-109">Uklonite sve adrese za prosleđivanje koje ne prepoznajete.</span><span class="sxs-lookup"><span data-stu-id="30b01-109">Remove any forwarding addresses you don't recognize.</span></span>