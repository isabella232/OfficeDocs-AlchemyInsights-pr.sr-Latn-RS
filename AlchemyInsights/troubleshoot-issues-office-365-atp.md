---
title: Rešavanje problema sa uslugom Office 365 napredna zaštita pretnje (ATP)
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
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758079"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="3d4a3-102">Rešavanje problema sa sistemom Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="3d4a3-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="3d4a3-103">**Primetite kašnjenje sa isporukom e-poruke**?</span><span class="sxs-lookup"><span data-stu-id="3d4a3-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="3d4a3-104">Pokušajte da koristite opciju dinamičko isporučivanje za ATP smernice bezbednih priloga.</span><span class="sxs-lookup"><span data-stu-id="3d4a3-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="3d4a3-105">To će izbeći da dolazi do kašnjenja e-poruke prilikom zaštite primalaca iz zlonamernog datoteka.</span><span class="sxs-lookup"><span data-stu-id="3d4a3-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="3d4a3-106">Da li **želite da prijavite lažne pozitivne ili lažne**negativne?</span><span class="sxs-lookup"><span data-stu-id="3d4a3-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="3d4a3-107">Koristite ovu povezanost da biste prosledili datoteku za analizu: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="3d4a3-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="3d4a3-108">Da **li ste znali da možete da omogućite ATP vezu bezbedne veze za e-poštu koje šalju osobe u organizaciji**?</span><span class="sxs-lookup"><span data-stu-id="3d4a3-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="3d4a3-109">Sledite ove korake:</span><span class="sxs-lookup"><span data-stu-id="3d4a3-109">Follow these steps:</span></span>
    1. <span data-ttu-id="3d4a3-110">Idite na i https://protection.office.com Prijavite se.</span><span class="sxs-lookup"><span data-stu-id="3d4a3-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="3d4a3-111">Smernice za **Upravljanje pretnjama**  >  **Policy**  >  **potražite bezbednim vezama**.</span><span class="sxs-lookup"><span data-stu-id="3d4a3-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="3d4a3-112">U okviru **smernice koje se primenjuju na određene primaoce**, uredite (ili dodajte) smernice.</span><span class="sxs-lookup"><span data-stu-id="3d4a3-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="3d4a3-113">Izaberite stavku **primenite bezbedne veze ka porukama poslatih unutar organizacije**.</span><span class="sxs-lookup"><span data-stu-id="3d4a3-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="3d4a3-114">Sačuvajte smernice i omogućite oko 30 minuta da promene prolaze kroz vaš put.</span><span class="sxs-lookup"><span data-stu-id="3d4a3-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="3d4a3-115">Da biste dobili dodatnu pomoć za ATP, pogledajte članak [Office 365 napredna zaštita pretnje](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="3d4a3-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>