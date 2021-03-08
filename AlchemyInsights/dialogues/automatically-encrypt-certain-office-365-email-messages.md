---
title: Automatsko šifrovanje određenih Office 365 e-poruka
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526740"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="f9e5b-102">Automatsko šifrovanje određenih Office 365 e-poruka</span><span class="sxs-lookup"><span data-stu-id="f9e5b-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="f9e5b-103">Možete automatski da šifrujete poruke koje korisnici šalju određenim spoljnim osobama ili organizacijama.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="f9e5b-104">Da biste to uradili, izvršite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="f9e5b-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="f9e5b-105">Iz [Exchange centra administracije](https://outlook.office365.com/ecp/)odaberite stavku **protok pošte > pravila**.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="f9e5b-106">Kliknite na **novu (+)** ikonu, a zatim izaberite stavku **primene Office 365 Message šifrovanje i zaštita prava na poruke**.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="f9e5b-107">U **ime** unesite ime pravila, kao što je *šifrovanje poruka koje se šalju u DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="f9e5b-108">U okviru **Primenjivanje ovog pravila ako**, odaberite **> primaoca ova osoba**.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="f9e5b-109">U prozoru **Izbor članova** izaberite ime osobe na koju želite da se prijavi šifrovanje, a zatim kliknite na dugme **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="f9e5b-110">Kada završite sa dodavanjem korisnika, kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="f9e5b-111">Pored polja **uradi sledeće** , izaberite stavku **Izaberi jednu**.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="f9e5b-112">U padajućem meniju **RMS predloška** izaberite stavku **šifrovanje**, a zatim kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="f9e5b-113">(Ako ne vidite ovu opciju, to znači da vaš plan ne podrazumeva automatsko šifrovanje.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="f9e5b-114">Ali možete da ga dodate!)</span><span class="sxs-lookup"><span data-stu-id="f9e5b-114">But you can add it!)</span></span>
9. <span data-ttu-id="f9e5b-115">Odaberite opcionalnu selekciju (sa liste opcionalnih izbora koje možete da napravite u ovom momentu, od kojih se mnogi mogu ostaviti podrazumevanom postavkom za jednostavnost).</span><span class="sxs-lookup"><span data-stu-id="f9e5b-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="f9e5b-116">Kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f9e5b-117">Uvek možete da se vratite i uredite ovo pravilo kasnije.</span><span class="sxs-lookup"><span data-stu-id="f9e5b-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="f9e5b-118">Više informacija o kreiranju pravila za šifrovanje potražite u članku [Definisanje pravila toka pošte za šifrovanje e-poruka u sistemu Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="f9e5b-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

