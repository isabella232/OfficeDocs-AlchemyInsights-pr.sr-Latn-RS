---
title: Omogućavanje upravljanja troškovima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678770"
---
# <a name="enable-cost-management"></a><span data-ttu-id="decea-102">Omogućavanje upravljanja troškovima</span><span class="sxs-lookup"><span data-stu-id="decea-102">Enable cost management</span></span>

<span data-ttu-id="decea-103">**Šta su to "Troškovi su onemogućili za vašu organizaciju"?**</span><span class="sxs-lookup"><span data-stu-id="decea-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="decea-104">Organizacije koje koriste Enterprise ugovor (EA) ili Microsoft ugovor sa klijentom (MCA) mogu da onemogućavaju pristup informacijama o troškovima i informacije o cijenama.</span><span class="sxs-lookup"><span data-stu-id="decea-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="decea-105">Kada se prijavite na Azure portal, oni mogu da koriste API-ove naplate da bi programski dobili fakture (kada se opozivaju) i detalji o korišćenju.</span><span class="sxs-lookup"><span data-stu-id="decea-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="decea-106">**Kako da omogućite dodatnim korisnicima da pristupe fakturama**</span><span class="sxs-lookup"><span data-stu-id="decea-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="decea-107">Idite na **oљtricu pretplate** u Azure portal.</span><span class="sxs-lookup"><span data-stu-id="decea-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="decea-108">Izaberite stavku **fakture** , a zatim **pristup fakturama**.</span><span class="sxs-lookup"><span data-stu-id="decea-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="decea-109">Uključite pristup, a zatim Čujte promene da biste korisnicima omogućili da u pretplati pretplate preuzmu fakture.</span><span class="sxs-lookup"><span data-stu-id="decea-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="decea-110">Administrator naloga može i da konfiguriše da se fakture šalju putem e-pošte.</span><span class="sxs-lookup"><span data-stu-id="decea-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="decea-111">Da biste saznali više, pogledajte članak [Nabavite fakturu putem e-pošte](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="decea-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="decea-112">**Kako da dodate korisnike ulozi čitača naplate**</span><span class="sxs-lookup"><span data-stu-id="decea-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="decea-113">Idite na **oљtricu pretplate** u Azure portal.</span><span class="sxs-lookup"><span data-stu-id="decea-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="decea-114">Izaberite stavku **Kontrola pristupa (IAM)** , a zatim kliknite na dugme **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="decea-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="decea-115">Odaberite stavku **čitač naplate** na stranici **Izbor uloge** .</span><span class="sxs-lookup"><span data-stu-id="decea-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="decea-116">Otkucajte e-poruku korisnika kojeg želite da pozovete, a zatim kliknite na dugme **u redu** da biste poslali poziv.</span><span class="sxs-lookup"><span data-stu-id="decea-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="decea-117">Pratićete uputstva navedena u porukama o pozivu da biste se prijavili kao čitač naplate.</span><span class="sxs-lookup"><span data-stu-id="decea-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="decea-118">Više informacija potražite u članku [Odobravanje pristupa naplata](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="decea-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="decea-119">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="decea-119">**Recommended documents**</span></span>

- [<span data-ttu-id="decea-120">Omogućavanje DA i AO prikaza putem EU portala</span><span class="sxs-lookup"><span data-stu-id="decea-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="decea-121">Troškovi koji su uključeni u upravljanje troškovima</span><span class="sxs-lookup"><span data-stu-id="decea-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="decea-122">Podržani Microsoft Azure ponude</span><span class="sxs-lookup"><span data-stu-id="decea-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="decea-123">Pregled troškova u analizi troška</span><span class="sxs-lookup"><span data-stu-id="decea-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="decea-124">Obezbeđivanje pristupa informacijama o plaćanju</span><span class="sxs-lookup"><span data-stu-id="decea-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="decea-125">Proveravaj pristup Microsoft ugovoru o klijentu</span><span class="sxs-lookup"><span data-stu-id="decea-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






