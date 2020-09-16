---
title: Kreiranje smernica nalepnica za AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732189"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="3981e-102">Kreiranje smernica nalepnica za AIP</span><span class="sxs-lookup"><span data-stu-id="3981e-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="3981e-103">Oznake Azure zaštite informacija (AIP) mogu se koristiti sa punim opsegom podataka koje organizacija najčešće kreira i skladišti, od najniže klasifikacije ličnih podataka, do najvišeg klasifikacije vrlo poverljivih podataka.</span><span class="sxs-lookup"><span data-stu-id="3981e-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="3981e-104">Smernice za zaštitu informacija o Azure postavkama primenjuju se na Classic klijent za Azure informacije (AIP), a ne na  [Aip Ujedinjenog označavanja klijenta](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="3981e-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="3981e-105">Možete da konfigurišete više elemenata u AIP smernicama, uključujući opcije kao što su:</span><span class="sxs-lookup"><span data-stu-id="3981e-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="3981e-106">Opcija za koju oznaku će dozvoliti administratorima ili klasifikaciju korisnika i e-porukama za zaštitu (opcionalno)</span><span class="sxs-lookup"><span data-stu-id="3981e-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="3981e-107">Opcija za nametanje klasifikacije kada korisnici čuvaju dokumente i šalju e-poštu</span><span class="sxs-lookup"><span data-stu-id="3981e-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="3981e-108">Opcija za automatsko označavanje e-poruke na osnovu njegovih priloga.</span><span class="sxs-lookup"><span data-stu-id="3981e-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="3981e-109">Opcija za kontrolisanje toga da li se traka za zaštitu informacija prikazuje u Office aplikacijama</span><span class="sxs-lookup"><span data-stu-id="3981e-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="3981e-110">Dodatne opcije i informacije o smernicama za zaštitu od Azure informacija potražite u članku: [Pregled smernica za zaštitu Azure informacija](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="3981e-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="3981e-111">Za druge korisne resurse u vezi sa AIP smernicama pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="3981e-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="3981e-112">Uputstvo: konfigurisanje Azure postavki smernica za zaštitu informacija i kreiranje nove nalepnice</span><span class="sxs-lookup"><span data-stu-id="3981e-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="3981e-113">Konfigurisanje smernica za zaštitu Azure informacija</span><span class="sxs-lookup"><span data-stu-id="3981e-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="3981e-114">Kreiranje i konfigurisanje nalepnica sa senzitivnošću i njihove smernice</span><span class="sxs-lookup"><span data-stu-id="3981e-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="3981e-115">Vodiča za uobičajene scenarije koji koriste Azure zaštitu informacija</span><span class="sxs-lookup"><span data-stu-id="3981e-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="3981e-116">Redigovanje dokumentacije za zaštitu informacija o Azure</span><span class="sxs-lookup"><span data-stu-id="3981e-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="3981e-117">Zahtevi za zaštitu Azure informacija</span><span class="sxs-lookup"><span data-stu-id="3981e-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="3981e-118">Brzi početak za uputstvo za Azure zaštitu informacija</span><span class="sxs-lookup"><span data-stu-id="3981e-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="3981e-119">Preuzimanje klijenta za zaštitu Azure informacija</span><span class="sxs-lookup"><span data-stu-id="3981e-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)