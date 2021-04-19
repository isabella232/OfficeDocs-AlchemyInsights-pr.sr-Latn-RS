---
title: 'AIP skener: instalacija i konfiguracija'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821677"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="3f00e-102">AIP skener: instalacija i konfiguracija</span><span class="sxs-lookup"><span data-stu-id="3f00e-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="3f00e-103">**Da biste instalirali AIP skener, pratite preporučena uputstva:**</span><span class="sxs-lookup"><span data-stu-id="3f00e-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="3f00e-104">Ako vršite nadogradnju i ne izvršavate čistu instalaciju, proverite da li ste pratili uputstva za nadogradnju [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) skenera, a za klijenta za oznake koji ima više oznaka, pogledajte nadogradnju [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)skenera.</span><span class="sxs-lookup"><span data-stu-id="3f00e-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="3f00e-105">Proverite da li ste usavršni sa svim [zahtevima postavki zaštitnih zidova i mrežne infrastrukture.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="3f00e-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="3f00e-106">Uverite se [da su smernice podešene na](https://docs.microsoft.com/azure/information-protection/configure-policy) automatsko označavanje ili da imaju podrazumevanu oznaku u smernicama.</span><span class="sxs-lookup"><span data-stu-id="3f00e-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="3f00e-107">Proverite da li je odgovarajući tip datoteke konfigurisan za oznaku/zaštitu kao što je opisano u članku Tipovi datoteka koje podržava [Azure Information Protection klijent.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="3f00e-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="3f00e-108">Pored toga, ako želite da promenite podrazumevano ponašanje, pratite ova uputstva: Promena podrazumevanog [nivoa zaštite datoteka.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="3f00e-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="3f00e-109">Proverite da li korisnički nalog konfigurisan za pokretanje usluge skenera ima dozvole za pristup svim konfigurisanim repositovima.</span><span class="sxs-lookup"><span data-stu-id="3f00e-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="3f00e-110">Ako i dalje imate problema, izvezite evidencije skenera i dodajte ih u tiket za podršku.</span><span class="sxs-lookup"><span data-stu-id="3f00e-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="3f00e-111">**Izvoz evidencija Azure Information Protection skenera**</span><span class="sxs-lookup"><span data-stu-id="3f00e-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="3f00e-112">Pređu na %localappdata%\Microsoft\MSIP u okviru korisničkog konteksta koji koristi uslugu skenera.</span><span class="sxs-lookup"><span data-stu-id="3f00e-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="3f00e-113">Zipuj sav sadržaj u fascikli MSIP.</span><span class="sxs-lookup"><span data-stu-id="3f00e-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="3f00e-114">Sačuvajte evidencije na svojoj lokaciji i priložite ih zahtevu za uslugom.</span><span class="sxs-lookup"><span data-stu-id="3f00e-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="3f00e-115">Možete da koristite [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="3f00e-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="3f00e-116">**Dodatne informacije potražite u:**</span><span class="sxs-lookup"><span data-stu-id="3f00e-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="3f00e-117">Primena Azure Information Protection skenera za automatsko klasifikaciju i zaštitu datoteka</span><span class="sxs-lookup"><span data-stu-id="3f00e-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="3f00e-118">Navođenje i korišćenje parametra tokena za set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="3f00e-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="3f00e-119">Pokretanje ciklusa otkrivanja i prikaz izveštaja za skener</span><span class="sxs-lookup"><span data-stu-id="3f00e-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="3f00e-120">Pregled dokumentacije za Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="3f00e-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="3f00e-121">Zahtevi za Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="3f00e-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="3f00e-122">Preuzimanje Azure Information Protection klijenta</span><span class="sxs-lookup"><span data-stu-id="3f00e-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
