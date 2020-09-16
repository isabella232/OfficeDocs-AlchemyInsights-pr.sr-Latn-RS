---
title: Odlazna e-pošta u fasciklu neželjene e-pošte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769197"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="af7d2-102">Odlazna e-pošta u fasciklu neželjene e-pošte</span><span class="sxs-lookup"><span data-stu-id="af7d2-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="af7d2-103">Ako vidite da su odlazne poruke označene kao neželjena, uradite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="af7d2-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="af7d2-104">Ako to već niste uradili, razmislite o [konfigurisanju obaveštenja o smernicama odlazne bezvredne pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="af7d2-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="af7d2-105">Koristite [praćenje poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) da biste videli da li izlazna poruka ima vrednost **bezvredne** manifestacije sa dodatnim detaljima: **Korišćenje bazena visokog rizika**.</span><span class="sxs-lookup"><span data-stu-id="af7d2-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="af7d2-106">Za ove poruke potvrdite sadržaj poruke da biste videli šta se može smatrati bezvredne.</span><span class="sxs-lookup"><span data-stu-id="af7d2-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="af7d2-107">Na primer, potpisi ponekad mogu da dovedu do problema za mnoge korisnike.</span><span class="sxs-lookup"><span data-stu-id="af7d2-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="af7d2-108">Ako imate više primera legitimnih izlaznih poruka koje su označene kao neželjene, otvorite ulaznicu za podršku i zatražite od agenta za podršku da prosledi poruke kao lažne pozitivne stvari našim pošiljaoca.</span><span class="sxs-lookup"><span data-stu-id="af7d2-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="af7d2-109">Pripremite se za obezbeđivanje uzoraka poruka koje sadrže sva zaglavlja poruka.</span><span class="sxs-lookup"><span data-stu-id="af7d2-109">Be prepared to provide sample messages that include all message headers.</span></span>
