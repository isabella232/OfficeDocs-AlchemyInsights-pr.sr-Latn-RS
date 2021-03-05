---
title: Blokiranje potpisa korisnika e-pošte
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483367"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="699ed-102">Blokiranje potpisa korisnika e-pošte</span><span class="sxs-lookup"><span data-stu-id="699ed-102">Block user-made email signatures</span></span>

<span data-ttu-id="699ed-103">Sledeće rešenje primenjuje se na potpise e-pošte kreiranim u programu Outlook na vebu.</span><span class="sxs-lookup"><span data-stu-id="699ed-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="699ed-104">Možete da blokirate samo potpise u Outlook aplikaciji ako imate lokalni Exchange server.</span><span class="sxs-lookup"><span data-stu-id="699ed-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="699ed-105">U centru administracije odaberite stavku **administrativni centri**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="699ed-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="699ed-106">Izaberite stavku **dozvole** za  >  **Outlook Web App smernice**.</span><span class="sxs-lookup"><span data-stu-id="699ed-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="699ed-107">Izaberite smernice, a zatim kliknite na ikonu olovke da biste je uredili.</span><span class="sxs-lookup"><span data-stu-id="699ed-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="699ed-108">Izaberite stavku **funkcije**  >  **Više opcija**.</span><span class="sxs-lookup"><span data-stu-id="699ed-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="699ed-109">U okviru **iskustvo korisnika** opozovite izbor u polju za potvrdu **potpis e-pošte** , a zatim kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="699ed-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="699ed-110">**Važno:** Ako je potpis dodat pre nego što opozovete izbor u ovom polju za potvrdu, korisnik će i dalje moći da ga koristi.</span><span class="sxs-lookup"><span data-stu-id="699ed-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="699ed-111">Zamolite ih da je uklone.</span><span class="sxs-lookup"><span data-stu-id="699ed-111">Ask them to remove it.</span></span>
