---
title: Rešavanje smernica veze
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750602"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="140c9-102">Rešavanje smernica veze</span><span class="sxs-lookup"><span data-stu-id="140c9-102">Fix connection policy</span></span>

<span data-ttu-id="140c9-103">E-poruka je označena kao bezbedna i isporučena u korisnički prijemno poštansko sanduče jer je IP adresa slanja označena kao bezbedna u smernicama za filtriranje veze.</span><span class="sxs-lookup"><span data-stu-id="140c9-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="140c9-104">Da biste pregledali smernice, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="140c9-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="140c9-105">Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim idite na smernice **za upravljanje pretnjama** za  >    >  [borbu protiv bezvredne pošte](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="140c9-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="140c9-106">Na kartici **Prilagođeno** izaberite **smernice za filtriranje veze**, a zatim izaberite stavku **Uredi smernice**.</span><span class="sxs-lookup"><span data-stu-id="140c9-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="140c9-107">Pregledajte listu **dozvole za IP** .</span><span class="sxs-lookup"><span data-stu-id="140c9-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="140c9-108">Pogledajte članak da li je **Sigurnosna lista** omogućena.</span><span class="sxs-lookup"><span data-stu-id="140c9-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="140c9-109">Microsoft se pretplate na nezavisne pošiljaoce pouzdanih pošiljalaca.</span><span class="sxs-lookup"><span data-stu-id="140c9-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="140c9-110">Ako je **bezbedna lista** omogućena, ovi pouzdani pošiljaoci nisu pogrešno označeni kao spam.</span><span class="sxs-lookup"><span data-stu-id="140c9-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="140c9-111">Preporuиujem vam da izaberete ovu opciju jer će se smanjiti broj pogrešnih informacija (dobra pošta koja je klasifikovana kao bezvredna pošta) koju primate.</span><span class="sxs-lookup"><span data-stu-id="140c9-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
