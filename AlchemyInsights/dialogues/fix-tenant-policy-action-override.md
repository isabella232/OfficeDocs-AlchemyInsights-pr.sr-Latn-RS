---
title: Popravka smernica zakupca (zamena radnje)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695695"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="1314a-102">Popravka smernica zakupca (zamena radnje)</span><span class="sxs-lookup"><span data-stu-id="1314a-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="1314a-103">Smernice za borbu protiv bezvredne pošte u zakupcu su pogođene ovom porukom.</span><span class="sxs-lookup"><span data-stu-id="1314a-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="1314a-104">Da biste pregledali smernice, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="1314a-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="1314a-105">Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim idite na smernice **za upravljanje pretnjama** za  >    >  [borbu protiv bezvredne pošte](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="1314a-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="1314a-106">Potvrdite izbor u polju za proveru da li **izvor smernica** ukazuje na sledeće:  **Add-Xzaglavlje/ModifySubject/preusmeri/Izbriši/bez radnje/Bcc poruka**</span><span class="sxs-lookup"><span data-stu-id="1314a-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="1314a-107">Ako je tako, na kartici **Prilagođeno** potvrdite postavke smernica koje utiču na poruku.</span><span class="sxs-lookup"><span data-stu-id="1314a-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="1314a-108">Moguće je da su **standardne postavke** koje su primene na sve korisnike Exchange online zaštitnog klijenta pogođene porukom.</span><span class="sxs-lookup"><span data-stu-id="1314a-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="1314a-109">Više informacija o konfigurisanju smernica za filtriranje bezvredne pošte potražite u članku [Konfigurisanje smernica za filtriranje bezvredne pošte](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="1314a-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
