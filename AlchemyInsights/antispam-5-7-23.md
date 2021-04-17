---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821425"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="d155a-102">Rešavanje problema sa isporukom e-pošte za kôd greške 5.7.23</span><span class="sxs-lookup"><span data-stu-id="d155a-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="d155a-103">Verifikujte SPF DNS zapis za domen u javno dostupnom kontroloru SPF ili DNS zapisa na vebu.</span><span class="sxs-lookup"><span data-stu-id="d155a-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="d155a-104">Potvrdite da Odlazna poruka nije identifikovana kao bezedna pošiljka od strane korporacije Microsoft i da je usmerena kroz prostor za isporuke visokog [rizika.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="d155a-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="d155a-105">Poruke u grupama za isporuku visokog rizika neće prođeti SPF provere i zbog toga odredišna organizacija e-pošte neće prihvatiti poruke.</span><span class="sxs-lookup"><span data-stu-id="d155a-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="d155a-106">Ako ponovo problem potraje, možda ćete morati da se obratite administratoru hosta pošte kom pokušavate da pošaljete e-poštu.</span><span class="sxs-lookup"><span data-stu-id="d155a-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="d155a-107">Napravite e-poruku o detaljnoj spoljnoj grešci koja je dostupna u poruci o neiskidanju.</span><span class="sxs-lookup"><span data-stu-id="d155a-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="d155a-108">Microsoft podrška možda neće moći dodatno da pomogne.</span><span class="sxs-lookup"><span data-stu-id="d155a-108">Microsoft support may not be able to assist further.</span></span>
