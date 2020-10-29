---
title: Rešavanje problema sa programom Microsoft Defender za Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801421"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="5574d-102">Rešavanje problema sa sistemom Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="5574d-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="5574d-103">**Primetite kašnjenje sa isporukom e-poruke** ?</span><span class="sxs-lookup"><span data-stu-id="5574d-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="5574d-104">Pokušajte da koristite opciju dinamičko isporučivanje za ATP smernice bezbednih priloga.</span><span class="sxs-lookup"><span data-stu-id="5574d-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="5574d-105">To će izbeći da dolazi do kašnjenja e-poruke prilikom zaštite primalaca iz zlonamernog datoteka.</span><span class="sxs-lookup"><span data-stu-id="5574d-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="5574d-106">Da li **želite da prijavite lažne pozitivne ili lažne** negativne?</span><span class="sxs-lookup"><span data-stu-id="5574d-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="5574d-107">Koristite ovu povezanost da biste prosledili datoteku za analizu: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="5574d-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="5574d-108">Da **li ste znali da možete da omogućite ATP vezu bezbedne veze za e-poštu koje šalju osobe u organizaciji** ?</span><span class="sxs-lookup"><span data-stu-id="5574d-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="5574d-109">Sledite ove korake:</span><span class="sxs-lookup"><span data-stu-id="5574d-109">Follow these steps:</span></span>
    1. <span data-ttu-id="5574d-110">Idite na i https://protection.office.com Prijavite se.</span><span class="sxs-lookup"><span data-stu-id="5574d-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="5574d-111">Smernice za **Upravljanje pretnjama**  >  **Policy**  >  **potražite bezbednim vezama** .</span><span class="sxs-lookup"><span data-stu-id="5574d-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="5574d-112">U okviru **smernice koje se primenjuju na određene primaoce** , uredite (ili dodajte) smernice.</span><span class="sxs-lookup"><span data-stu-id="5574d-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="5574d-113">Izaberite stavku **primenite bezbedne veze ka porukama poslatih unutar organizacije** .</span><span class="sxs-lookup"><span data-stu-id="5574d-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="5574d-114">Sačuvajte smernice i omogućite oko 30 minuta da promene prolaze kroz vaš put.</span><span class="sxs-lookup"><span data-stu-id="5574d-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="5574d-115">Da biste dobili veću pomoć za ATP, pogledajte članak [Microsoft zaštitnik za Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="5574d-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>