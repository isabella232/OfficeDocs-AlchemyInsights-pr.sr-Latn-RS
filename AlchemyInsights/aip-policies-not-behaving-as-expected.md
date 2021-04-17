---
title: 'AIP: Smernice se ne ponašaju kao što se očekuje'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821641"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="5f3c6-102">AIP: Smernice se ne ponašaju kao što se očekuje</span><span class="sxs-lookup"><span data-stu-id="5f3c6-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="5f3c6-103">Azure Information Protection: Smernice koje se ne ponašaju kao što se očekuje, pogledajte sledeće da biste dobili preporučena uputstva za različite probleme sa smernicama:</span><span class="sxs-lookup"><span data-stu-id="5f3c6-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="5f3c6-104">Ako imate problema sa vizuelnim oznakama, pregledajte kada [se primenjuju vizuelne oznake.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="5f3c6-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="5f3c6-105">Ako imate problema sa automatskom oznakom, pogledajte kako da konfigurišete uslove za automatsku i preporučenu klasifikaciju za [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Šta tipovi osetljivih [informacija potraže.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="5f3c6-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="5f3c6-106">Ako imate problema sa zaštitom native/Pfile, pregledajte [konfiguraciju API-ja datoteke.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="5f3c6-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="5f3c6-107">Proverite da li koristite određivane smernice koje nisu ispravno konfigurisane: Kako se konfiguriše [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)smernica za određene korisnike pomoću proširenih smernica.</span><span class="sxs-lookup"><span data-stu-id="5f3c6-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="5f3c6-108">Ako automatsko označavanje ne funkcioniše za Outlook kada prilažete označeni dokument, proverite da DRMEncryptProperty nije definisan kao što je opisano ovde: Postavke [IRM registratora](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)za bezbednost.</span><span class="sxs-lookup"><span data-stu-id="5f3c6-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="5f3c6-109">Ako i dalje imate problema, prikupite evidencije Azure Information Protection klijenta i priložite izvezene evidencije ovom tiketu.</span><span class="sxs-lookup"><span data-stu-id="5f3c6-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="5f3c6-110">Otvorite Office dokument ili kreirajte novu e-poruku u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="5f3c6-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="5f3c6-111">Izaberite **stavku Pomoć i povratne informacije o**  >  **zaštiti/osetljivosti.**</span><span class="sxs-lookup"><span data-stu-id="5f3c6-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="5f3c6-112">Izaberite **stavku Izvoz evidencija**.</span><span class="sxs-lookup"><span data-stu-id="5f3c6-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="5f3c6-113">Sačuvajte evidencije na svojoj lokaciji i priložite ih ovom zahtevu za uslugom.</span><span class="sxs-lookup"><span data-stu-id="5f3c6-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="5f3c6-114">Dodatni resursi:</span><span class="sxs-lookup"><span data-stu-id="5f3c6-114">Additional resources:</span></span>

- [<span data-ttu-id="5f3c6-115">Konfigurisanje oznake za vizuelne oznake za Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="5f3c6-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="5f3c6-116">Pregled dokumentacije za Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="5f3c6-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="5f3c6-117">Korišćenje oznaka osetljivosti u Microsoft 365 aplikacijama</span><span class="sxs-lookup"><span data-stu-id="5f3c6-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

