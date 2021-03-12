---
title: Primer Microsoft Defender za Office 365 smernice za bezbedne priloge
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749198"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="1b3f2-102">Primer Microsoft Defender za Office 365 smernice za bezbedne priloge</span><span class="sxs-lookup"><span data-stu-id="1b3f2-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="1b3f2-103">Ove postavke omogućavaju smernice pod imenom *bez kašnjenja* koje odmah šalju poruke, a zatim ponovo prilaže priloge posle skeniranja:</span><span class="sxs-lookup"><span data-stu-id="1b3f2-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="1b3f2-104">**Ime**: nema kašnjenja</span><span class="sxs-lookup"><span data-stu-id="1b3f2-104">**Name**: No delays</span></span>
- <span data-ttu-id="1b3f2-105">**Opis**: dostavlja poruke odmah i ponovo prilaže priloge posle skeniranja.</span><span class="sxs-lookup"><span data-stu-id="1b3f2-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="1b3f2-106">**Odgovor**: izaberite opciju **Dinamičko** rešenje.</span><span class="sxs-lookup"><span data-stu-id="1b3f2-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="1b3f2-107">Više informacija potražite u članku [Dinamičko isporučivanje u smernicama bezbednog priloga](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="1b3f2-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="1b3f2-108">Odeljak " **Preusmeravanje priloga** ": izaberite opciju **Omogućavanje preusmeravanja**, a zatim unesite e-adresu Microsoft 365 globalnog administratora, administratora bezbednosti ili analitičara koji će istražiti zlonamerne priloge.</span><span class="sxs-lookup"><span data-stu-id="1b3f2-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="1b3f2-109">**Primeni na** odeljak: izaberite **domen primaoca**, a zatim izaberite domen.</span><span class="sxs-lookup"><span data-stu-id="1b3f2-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="1b3f2-110">Izaberite stavku **Dodaj**, a zatim kliknite na **dugme u redu**.</span><span class="sxs-lookup"><span data-stu-id="1b3f2-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="1b3f2-111">Kada završite, izaberite stavku **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="1b3f2-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="1b3f2-112">Da biste saznali više, pogledajte odeljak [bezbedni prilozi u programu Microsoft zaštitnik za Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="1b3f2-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
