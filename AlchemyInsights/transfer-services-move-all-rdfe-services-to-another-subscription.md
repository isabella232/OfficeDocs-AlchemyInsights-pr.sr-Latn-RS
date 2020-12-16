---
title: Prenos usluga – premeštanje svih RDFE usluga na drugu pretplatu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692175"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="5f1a7-102">Prenos usluga – premeštanje svih RDFE usluga na drugu pretplatu</span><span class="sxs-lookup"><span data-stu-id="5f1a7-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="5f1a7-103">**Premeštanje resursa**</span><span class="sxs-lookup"><span data-stu-id="5f1a7-103">**Move resources**</span></span>

<span data-ttu-id="5f1a7-104">Azure resursi mogu da se premeštaju u drugu Azure pretplatu ili grupu resursa u okviru iste pretplate pomoću Azure portala, Azure PowerShell, Azure CLI ili OSTATAK API-ja za premeštanje resursa.</span><span class="sxs-lookup"><span data-stu-id="5f1a7-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="5f1a7-105">Da biste mogli da premestite resurse, pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="5f1a7-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="5f1a7-106">Kontrolna lista pre premeštanja resursa</span><span class="sxs-lookup"><span data-stu-id="5f1a7-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="5f1a7-107">Usluge koje mogu da se premeste</span><span class="sxs-lookup"><span data-stu-id="5f1a7-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="5f1a7-108">Kako da proverite valjanost premeštanja</span><span class="sxs-lookup"><span data-stu-id="5f1a7-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="5f1a7-109">Premeštanje smernica za usluge</span><span class="sxs-lookup"><span data-stu-id="5f1a7-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="5f1a7-110">Da biste premestili postojeće resurse u drugu grupu resursa ili pretplatu, možete da koristite:</span><span class="sxs-lookup"><span data-stu-id="5f1a7-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="5f1a7-111">Azure portal</span><span class="sxs-lookup"><span data-stu-id="5f1a7-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="5f1a7-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="5f1a7-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="5f1a7-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5f1a7-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="5f1a7-114">REST API</span><span class="sxs-lookup"><span data-stu-id="5f1a7-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="5f1a7-115">Uputstvo: [Premeštanje Azure resursa u drugu grupu resursa ili pretplatu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="5f1a7-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="5f1a7-116">**Rešavanje problema sa greškama u alatki Azure Manager**</span><span class="sxs-lookup"><span data-stu-id="5f1a7-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="5f1a7-117">Pogledajte članke ispod da biste saznali više o uobičajenim Azure greškama prilikom raspoređivanja i primite informacije za njih.</span><span class="sxs-lookup"><span data-stu-id="5f1a7-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="5f1a7-118">Ako ne možete da pronađete kôd greške za vašu grešku prilikom primene, pogledajte članak [Pronalaženje kôda greške](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="5f1a7-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="5f1a7-119">Rešavanje problema sa ispravkom primene</span><span class="sxs-lookup"><span data-stu-id="5f1a7-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="5f1a7-120">Rešavanje problema pri premeštanju Azure resursa u novu grupu resursa ili pretplatu</span><span class="sxs-lookup"><span data-stu-id="5f1a7-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="5f1a7-121">Imajte u vidu da ako želite da nadogradite Azure pretplatu, kao što je prebacivanje sa slobodne na Pay-as-go, moraćete da konvertujete pretplatu.</span><span class="sxs-lookup"><span data-stu-id="5f1a7-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="5f1a7-122">Da biste nadogradili besplatnu probnu verziju, pogledajte članak [Nadogradnja besplatnog pokušaja ili Microsoft pogledajte Azure pretplatu na "pay-as](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)".</span><span class="sxs-lookup"><span data-stu-id="5f1a7-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="5f1a7-123">Da biste promenili nalog za plaćanje plaćanja, pogledajte članak [Promena Azure Pay-as-you-go pretplate na drugačiju ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="5f1a7-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="5f1a7-124">**Da biste dodali ili povezali Azure pretplatu na Azure Active Directory stanar:**</span><span class="sxs-lookup"><span data-stu-id="5f1a7-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="5f1a7-125">Prijavite se i izaberite pretplatu koju želite da koristite na stranici " [pretplate" u usluzi Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="5f1a7-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="5f1a7-126">Izaberite stavku **Promeni direktorijum**.</span><span class="sxs-lookup"><span data-stu-id="5f1a7-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="5f1a7-127">Pregledajte sva upozorenja koja se pojavljuju, a zatim izaberite stavku **Promeni**.</span><span class="sxs-lookup"><span data-stu-id="5f1a7-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="5f1a7-128">Direktorijum se menja za pretplatu i imaćete poruku o uspehu.</span><span class="sxs-lookup"><span data-stu-id="5f1a7-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="5f1a7-129">Koristite sviščer *direktorijuma* da biste otiљli u novi direktorijum.</span><span class="sxs-lookup"><span data-stu-id="5f1a7-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="5f1a7-130">Može biti potrebno do 10 minuta da se sve dobro pokaže.</span><span class="sxs-lookup"><span data-stu-id="5f1a7-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="5f1a7-131">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="5f1a7-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="5f1a7-132">Prebacivanje vlasništva nad Azure pretplatom</span><span class="sxs-lookup"><span data-stu-id="5f1a7-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="5f1a7-133">Premeštanje resursa na novu grupu resursa ili pretplatu</span><span class="sxs-lookup"><span data-stu-id="5f1a7-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="5f1a7-134">Upravljanje resursima pomoću Azure portala</span><span class="sxs-lookup"><span data-stu-id="5f1a7-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
