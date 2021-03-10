---
title: Popravka postavki smernica za korisnike/poštansko sanduče
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695903"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="5059a-102">Popravka postavki smernica za korisnike/poštansko sanduče</span><span class="sxs-lookup"><span data-stu-id="5059a-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="5059a-103">Postavke neželjene pošte u poštanskom sandučetu utiču na ovu poruku.</span><span class="sxs-lookup"><span data-stu-id="5059a-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="5059a-104">Da biste pregledali postavke, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="5059a-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="5059a-105">Pokrenite Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="5059a-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="5059a-106">Više informacija potražite u članku [Otvaranje programskog dodatka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="5059a-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="5059a-107">Pokrene ovu komandu (pomoću e-adrese korisnika):  **uzmi-mailboxconfiguration mail Configuration-identitet "User@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="5059a-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="5059a-108">Potvrdite da li je adresa e-pošte pošiljaoca deo **poverendindersandždodomena** ili **blokiranih domena**.</span><span class="sxs-lookup"><span data-stu-id="5059a-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="5059a-109">Ako se e-adresa nalazi na jednoj od listi, možda ćete morati da je uklonite.</span><span class="sxs-lookup"><span data-stu-id="5059a-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="5059a-110">Da biste saznali više, pogledajte članak [Podešavanje konfiguracije-Mailboxjunkemailsanduče](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="5059a-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
