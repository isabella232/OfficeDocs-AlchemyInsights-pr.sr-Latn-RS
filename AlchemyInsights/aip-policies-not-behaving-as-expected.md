---
title: 'AIP: smernice se ne ponašaju po očekivanim'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663203"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="1d16c-102">AIP: smernice se ne ponašaju po očekivanim</span><span class="sxs-lookup"><span data-stu-id="1d16c-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="1d16c-103">Zaštita od Azure informacija: smernice se ne ponašaju po očekivanim, pogledajte sledeće za preporučene smernice za različite probleme sa politikom:</span><span class="sxs-lookup"><span data-stu-id="1d16c-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="1d16c-104">Ako imate problema sa vizuelnim oznakama, pregledajte [kada se primene vizuelne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="1d16c-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="1d16c-105">Ako imate problema sa automatskim označenjem, pregledajte [Kako da konfigurišete uslove za automatsku i preporučenu klasifikaciju za zaštitu Azure informacija](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i [Šta tipovi osetljivim informacija traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="1d16c-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="1d16c-106">Ako imate problema sa zaštitom od izvorne/Pfile zaštite, pregledajte [KONFIGURACIJU API datoteke](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="1d16c-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="1d16c-107">Potvrdite izbor u polju za proveru da li koristite ispravljene smernice koje nisu ispravno konfigurisane: [Kako da konfigurišete smernice za bezbednost Azure za određene korisnike pomoću](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)ispravljene polise.</span><span class="sxs-lookup"><span data-stu-id="1d16c-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="1d16c-108">Ako Automatsko označavanje ne radi za Outlook prilikom prilazavanja označenog dokumenta, proverite da li je svojstvo Drajmencryptdefinisano kao ovde opisano: [postavke registratora za bezbednost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="1d16c-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="1d16c-109">Ako i dalje imate problema, sakupite Azure klijentske zapise zaštite klijenata i priložite izvezene evidentira na ovu kartu.</span><span class="sxs-lookup"><span data-stu-id="1d16c-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="1d16c-110">Otvorite Office dokument ili kreirajte novu e-poruku u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="1d16c-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="1d16c-111">Izaberite stavku **Zaštita/osetljivost**  >  **pomoći i povratne informacije**.</span><span class="sxs-lookup"><span data-stu-id="1d16c-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="1d16c-112">Izaberite stavku **evidencija izvoza**.</span><span class="sxs-lookup"><span data-stu-id="1d16c-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="1d16c-113">Sačuvajte evidentira na svoj izbor lokacije i priložite ih na ovaj zahtev za uslugom.</span><span class="sxs-lookup"><span data-stu-id="1d16c-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="1d16c-114">Dodatni resursi:</span><span class="sxs-lookup"><span data-stu-id="1d16c-114">Additional resources:</span></span>

- [<span data-ttu-id="1d16c-115">Kako da konfigurišete oznaku za vizuelne oznake za Azure informacionu zaštitu</span><span class="sxs-lookup"><span data-stu-id="1d16c-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="1d16c-116">Redigovanje dokumentacije za zaštitu informacija o Azure</span><span class="sxs-lookup"><span data-stu-id="1d16c-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="1d16c-117">Korišćenje oznaka za osetljivost u Microsoft 365 aplikacijama</span><span class="sxs-lookup"><span data-stu-id="1d16c-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

