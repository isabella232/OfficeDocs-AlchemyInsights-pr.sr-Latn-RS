---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717339"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="ba3a6-102">Rešavanje problema sa isporukom e-pošte za kôd greške 5.7.23</span><span class="sxs-lookup"><span data-stu-id="ba3a6-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="ba3a6-103">Verifikujte program za SPF za vaš domen na javnom dostupnom kontroloru SPF ili DNS zapisima na vebu.</span><span class="sxs-lookup"><span data-stu-id="ba3a6-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="ba3a6-104">Potvrdite da Microsoft nije identifikovan kao bezvredna poruka i usmeren kroz [visoki prostor za isporuku rizika](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="ba3a6-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="ba3a6-105">Poruke u bazenu visokog rizika neće proći CIF provere i zato neće biti prihvaćeni od strane odredišta e-pošte.</span><span class="sxs-lookup"><span data-stu-id="ba3a6-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="ba3a6-106">Ako se problem ponavlja, možda ćete morati da se obratite administratoru domaćina pošte kojem pokušavate da pošaljete e-poruku.</span><span class="sxs-lookup"><span data-stu-id="ba3a6-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="ba3a6-107">Zabeležite detaljnu spoljašnju grešku dostupnu u poruci "iskakanja".</span><span class="sxs-lookup"><span data-stu-id="ba3a6-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="ba3a6-108">Microsoft Support možda neće moći da pomogne dalje.</span><span class="sxs-lookup"><span data-stu-id="ba3a6-108">Microsoft support may not be able to assist further.</span></span>
