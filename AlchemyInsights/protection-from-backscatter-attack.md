---
title: Zaštita od napada
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037177"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="5bd03-102">Zaštita od napada</span><span class="sxs-lookup"><span data-stu-id="5bd03-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="5bd03-103">Backscatfor nije izveštaji o isporuci (poznat i kao NDRs ili iskačuće poruke) koje primate za poruke koje niste poslali.</span><span class="sxs-lookup"><span data-stu-id="5bd03-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="5bd03-104">"Spammers Forge" (pojedini) **iz:** adresa svojih poruka, a one često koriste prave e-adrese da bi svojim porukama pozajmili kredibilitet.</span><span class="sxs-lookup"><span data-stu-id="5bd03-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="5bd03-105">Kada pošiljaoci bezvredne pošte neminovno šalju poruke nepostojećim primaocima, odredišni server e-pošte je u suљtini napravljen da vrati poruku o neisporučivanju u NDR za krivotvorenog pošiljaoca u **:** adresi.</span><span class="sxs-lookup"><span data-stu-id="5bd03-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="5bd03-106">Dodatne informacije mogu se pronaći u okviru [nazad u programu EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="5bd03-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="5bd03-107">**Omogućavanje zaštite**</span><span class="sxs-lookup"><span data-stu-id="5bd03-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="5bd03-108">Da biste omogućili zaštitu, uradite sledeće.</span><span class="sxs-lookup"><span data-stu-id="5bd03-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="5bd03-109">**protection.office.com > > smernica za upravljanje pretnjama > > izaberite smernice za filtriranje bezvredne pošte i uredite smernice > svojstva bezvredne > Označi kao bezvredne > NDR backscat> podesi na "uključeno"**</span><span class="sxs-lookup"><span data-stu-id="5bd03-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="5bd03-110">Ako smatrate da je nalog kompromitovan, pogledajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="5bd03-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="5bd03-111">Odgovaranje na kompromitovani nalog e-pošte</span><span class="sxs-lookup"><span data-stu-id="5bd03-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="5bd03-112">Uklanjanje blokiranih korisnika sa portala Limitenih korisnika u sistemu Office 365</span><span class="sxs-lookup"><span data-stu-id="5bd03-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



