---
title: Rešavanje problema sa programom Microsoft Defender za Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801457"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="7a1b4-102">Rešavanje problema sa programom Microsoft Defender za Office 365</span><span class="sxs-lookup"><span data-stu-id="7a1b4-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="7a1b4-103">Da li primečujete kašnjenje u isporuci poruka?</span><span class="sxs-lookup"><span data-stu-id="7a1b4-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="7a1b4-104">Koristite opciju [Dinamičko isporučivanje](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) u ATP smernicama bezbednih priloga.</span><span class="sxs-lookup"><span data-stu-id="7a1b4-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="7a1b4-105">To će vam pomoći da izbegnete kašnjenje poruke prilikom zaštite primalaca iz zlonamernog datoteka.</span><span class="sxs-lookup"><span data-stu-id="7a1b4-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="7a1b4-106">Da li želite da prijavite lažne pozitivne ili lažne negative korporaciji Microsoft?</span><span class="sxs-lookup"><span data-stu-id="7a1b4-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="7a1b4-107">Koristite ovu [povezanost](https://www.microsoft.com/wdsi/filesubmission/) za prosleđivanje datoteka za analizu.</span><span class="sxs-lookup"><span data-stu-id="7a1b4-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="7a1b4-108">Da li ste znali da možete da omogućite zaštitu bezbedne veze za unutrašnju e-poštu poslatih između primalaca iz vaše organizacije?</span><span class="sxs-lookup"><span data-stu-id="7a1b4-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="7a1b4-109">Sledite ove korake:</span><span class="sxs-lookup"><span data-stu-id="7a1b4-109">Follow these steps:</span></span>

  1. <span data-ttu-id="7a1b4-110">Idite na stavku [https://protection.office.com](https://protection.office.com) i prijavite se pomoću opšteg administratora ili administratorskog naloga.</span><span class="sxs-lookup"><span data-stu-id="7a1b4-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="7a1b4-111">U levom oknu za navigaciju u okviru stavke **Upravljanje pretnjama** **Odaberite stavku** \> **bezbedne veze** .</span><span class="sxs-lookup"><span data-stu-id="7a1b4-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="7a1b4-112">U **smernicama koje se primenjuju na ceo odeljak organizacije** izaberite smernice i izaberite stavku **Uredi** .</span><span class="sxs-lookup"><span data-stu-id="7a1b4-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="7a1b4-113">U okviru **Postavke** , omogućite **primenu bezbednih veza ka porukama poslatih unutar organizacije** .</span><span class="sxs-lookup"><span data-stu-id="7a1b4-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
