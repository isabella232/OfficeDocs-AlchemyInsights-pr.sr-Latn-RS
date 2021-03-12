---
title: Automatsko šifrovanje određenih e-poruka iz sistema Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749458"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="381c3-102">Automatsko šifrovanje određenih e-poruka iz sistema Office 365</span><span class="sxs-lookup"><span data-stu-id="381c3-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="381c3-103">Iz [Exchange centra administracije](https://outlook.office365.com/ecp/)odaberite stavku **protok pošte > pravila**.</span><span class="sxs-lookup"><span data-stu-id="381c3-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="381c3-104">Kliknite na **novu (+)** ikonu, a zatim izaberite stavku **primene Office 365 Message šifrovanje i zaštita prava na poruke**.</span><span class="sxs-lookup"><span data-stu-id="381c3-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="381c3-105">U **ime**, unesite ime za pravilo, kao što je *šifrovanje svih poruka*.</span><span class="sxs-lookup"><span data-stu-id="381c3-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="381c3-106">U okviru **Primenjivanje ovog pravila ako**, odaberite **[primenjuje se na sve poruke]**.</span><span class="sxs-lookup"><span data-stu-id="381c3-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="381c3-107">Pored polja **uradi sledeće** , izaberite stavku **Izaberi jednu**.</span><span class="sxs-lookup"><span data-stu-id="381c3-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="381c3-108">U padajućem meniju **RMS predloška** izaberite stavku **šifrovanje**, a zatim kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="381c3-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="381c3-109">(Ako ne vidite ovu opciju, to znači da vaš plan ne podrazumeva automatsko šifrovanje.</span><span class="sxs-lookup"><span data-stu-id="381c3-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="381c3-110">Ali možete da ga dodate!)</span><span class="sxs-lookup"><span data-stu-id="381c3-110">But you can add it!)</span></span>
7. <span data-ttu-id="381c3-111">Potvrdite izbor u polju za potvrdu **nadgledanje ovo pravilo pomoću nivoa ozbiljnosti** , a zatim izaberite željeni nivo.</span><span class="sxs-lookup"><span data-stu-id="381c3-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="381c3-112">Ako vaše preduzeće ima ugovorne obaveze za slanje svih šifrovanih e-poruka, preporuиujem podešavanje nivoa na **najviša**.</span><span class="sxs-lookup"><span data-stu-id="381c3-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="381c3-113">U okviru **Odaberite model za ovo pravilo** kliknite na dugme **Primeni**.</span><span class="sxs-lookup"><span data-stu-id="381c3-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="381c3-114">Odaberite opcionalnu selekciju (sa liste opcionalnih izbora koje možete da napravite u ovom momentu, od kojih se mnogi mogu ostaviti podrazumevanom postavkom za jednostavnost).</span><span class="sxs-lookup"><span data-stu-id="381c3-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="381c3-115">Kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="381c3-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="381c3-116">Uvek možete da se vratite i uredite ovo pravilo kasnije.</span><span class="sxs-lookup"><span data-stu-id="381c3-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="381c3-117">Više informacija o kreiranju pravila za šifrovanje potražite u članku [Definisanje pravila toka pošte za šifrovanje e-poruka u sistemu Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="381c3-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

