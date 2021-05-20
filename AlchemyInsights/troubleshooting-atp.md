---
title: Rešavanje problema sa microsoft zaštitnikom za Office 365
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545282"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="5948f-102">Rešavanje problema sa microsoft zaštitnikom za Office 365</span><span class="sxs-lookup"><span data-stu-id="5948f-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="5948f-103">**Da li ste primetili kašnjenja u isporuci poruke?**</span><span class="sxs-lookup"><span data-stu-id="5948f-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="5948f-104">Koristite [opciju Dinamička isporuka](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) u Programu Microsoft zaštitnik za Office 365 Sef za priloge.</span><span class="sxs-lookup"><span data-stu-id="5948f-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="5948f-105">To će pomoći da se izbegnu kašnjenja u porukama dok štitite primaoce od zlonamernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="5948f-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="5948f-106">**Želite li da korporaciji Microsoft prijavite pozitivne ili netačne negativne vrednosti?**</span><span class="sxs-lookup"><span data-stu-id="5948f-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="5948f-107">Koristite [Istraživač prosleđivanja](https://protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="5948f-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="5948f-108">-\*\* Da li ste znali da možete da omogućite Sef Zaštitu veza za internu e-poštu poslau između primalaca u vašoj organizaciji?\*\* Pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="5948f-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="5948f-109">Idite na nalog globalnog administratora ili administratora bezbednosti i [https://protection.office.com](https://protection.office.com) prijavite se sa njim.</span><span class="sxs-lookup"><span data-stu-id="5948f-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="5948f-110">U levom oknu za navigaciju, **u okviru Upravljanje pretnjama** **odaberite** \> **stavke Smernice Sef veze.**</span><span class="sxs-lookup"><span data-stu-id="5948f-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="5948f-111">U **odeljku Smernice koje se primenjuju na celu organizaciju** izaberite smernicu i kliknite na dugme **Uredi**.</span><span class="sxs-lookup"><span data-stu-id="5948f-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="5948f-112">U **Postavke** omogući primenu **bezbednih veza na poruke poslate u okviru organizacije**.</span><span class="sxs-lookup"><span data-stu-id="5948f-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
