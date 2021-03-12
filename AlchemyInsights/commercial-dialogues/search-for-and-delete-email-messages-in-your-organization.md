---
title: Pretraga i brisanje e-poruka u organizaciji
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750015"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="b1e1f-102">Pretraga i brisanje e-poruka u organizaciji</span><span class="sxs-lookup"><span data-stu-id="b1e1f-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="b1e1f-103">Sledite ove korake:</span><span class="sxs-lookup"><span data-stu-id="b1e1f-103">Follow these steps:</span></span>

1. <span data-ttu-id="b1e1f-104">Ako niste globalni administrator, da biste pretražili poruke, nalog mora biti dodat u **grupu uloga programa Ediscovery Manager** ili **ulogu upravljanja usaglašenosti**.</span><span class="sxs-lookup"><span data-stu-id="b1e1f-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="b1e1f-105">Da biste izbrisali poruke, moraćete da se pridružite **grupi uloga za upravljanje organizacijom** ili svojoj **ulozi za pretraživanje i čišćenje**.</span><span class="sxs-lookup"><span data-stu-id="b1e1f-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="b1e1f-106">Dozvole za ove uloge se dodeljuju u [centru za bezbednost & bezbednosti.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="b1e1f-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="b1e1f-107">[Kreirajte pretragu sadržaja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku za brisanje.</span><span class="sxs-lookup"><span data-stu-id="b1e1f-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="b1e1f-108">[Povezivanje sa bezbednosnim & PowerShell Center usaglašenosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b1e1f-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="b1e1f-109">Ako koristite MFA, pogledajte ova uputstva: [Povezivanje sa bezbednosnim & PowerShell Center za usaglašenost pomoću multifaktor potvrde identiteta](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="b1e1f-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="b1e1f-110">Izbriši poruku: Pokreće `New-ComplianceSearchAction` cmdlet da biste izbrisali poruku.</span><span class="sxs-lookup"><span data-stu-id="b1e1f-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="b1e1f-111">Izbrisane poruke se premeštaju u fasciklu "stavke koje se mogu spasti korisnik".</span><span class="sxs-lookup"><span data-stu-id="b1e1f-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="b1e1f-112">Za primer komande pogledajte odeljak [3: brisanje poruke.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="b1e1f-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
