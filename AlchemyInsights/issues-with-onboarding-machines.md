---
title: Problemi sa ulaznom migracijom računara u Microsoft zaštitnik za krajnje tačke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901581"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="402ad-102">Problemi sa ulaznom migracijom računara u Microsoft zaštitnik za krajnje tačke</span><span class="sxs-lookup"><span data-stu-id="402ad-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="402ad-103">Možda ćete imati problema sa ulaznom migracijom računara za MDE uslugu.</span><span class="sxs-lookup"><span data-stu-id="402ad-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="402ad-104">Ako možete da pristupite računaru krajnjih korisnika, pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="402ad-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="402ad-105">Preuzmite najnoviju verziju pregleda dijagnostičkog alata[MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="402ad-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="402ad-106">Kliknite desnim tasterom **MDEClientAnalyzer.cmd** i izaberite stavku "Pokreni kao administrator".</span><span class="sxs-lookup"><span data-stu-id="402ad-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="402ad-107">Pratite uputstva koja su predložena u **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="402ad-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="402ad-108">Za više detaljnih evidencija, pregledajte kreiranu potfasciklu pod imenom **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="402ad-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="402ad-109">Ako su potrebna dodatna uputstva, obratite se [podršci Microsoft zaštitnik za krajnju tačku](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) i dostavite dobijenu MDEClientAnalyzerResult.zip datoteku za analizu.</span><span class="sxs-lookup"><span data-stu-id="402ad-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
