---
title: Kreiranje smernica za AIP oznake
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569510"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="0eaea-102">Kreiranje smernica za AIP oznake</span><span class="sxs-lookup"><span data-stu-id="0eaea-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="0eaea-103">Oznake za zaštitu poverljivih informacija (AIP) mogu da se koriste sa celokupnim opsegom podataka koje organizacija obično kreira i skladišti, od najniže klasifikacije ličnih podataka, do najveće klasifikacije veoma poverljivih podataka.</span><span class="sxs-lookup"><span data-stu-id="0eaea-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="0eaea-104">Smernice za zaštitu informacija koje se odnose na Azure primenjuju se na Classic klijent za zaštitu informacija (AIP), a ne na [Aip](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="0eaea-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="0eaea-105">Možete da konfigurišete više elemenata u AIP smernici, uključujući opcije kao što su:</span><span class="sxs-lookup"><span data-stu-id="0eaea-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="0eaea-106">Opcija za koju će oznaka dopustiti administratorima ili korisnicima klasifikovati i zaštititi (opcionalno) dokumente i e-poruke</span><span class="sxs-lookup"><span data-stu-id="0eaea-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="0eaea-107">Opcija za primenu klasifikacije kada korisnici sačuvaju dokumente i šalju e-poruke</span><span class="sxs-lookup"><span data-stu-id="0eaea-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="0eaea-108">Opcija za automatsko označavanje e-poruke na osnovu njenih priloga.</span><span class="sxs-lookup"><span data-stu-id="0eaea-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="0eaea-109">Opcija za kontrolisanje da li je traka za zaštitu informacija prikazana u Office aplikacijama</span><span class="sxs-lookup"><span data-stu-id="0eaea-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="0eaea-110">Dodatne opcije i informacije o smernicama za zaštitu od Azure informacija potražite u članku: [Pregled smernica za zaštitu od Azure informacija](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="0eaea-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="0eaea-111">Za druge korisne resurse vezane za AIP smernice pogledajte:</span><span class="sxs-lookup"><span data-stu-id="0eaea-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="0eaea-112">Uputstvo: konfigurisanje Azure postavki smernica za zaštitu informacija i kreiranje nove nalepnice</span><span class="sxs-lookup"><span data-stu-id="0eaea-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="0eaea-113">Konfigurisanje smernica za zaštitu informacija o Azure podacima</span><span class="sxs-lookup"><span data-stu-id="0eaea-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="0eaea-114">Kreiranje i Podešavanje oznaka osetljivosti i njihovih smernica</span><span class="sxs-lookup"><span data-stu-id="0eaea-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="0eaea-115">Vodiči za uobičajene scenarije koji koriste Azure zaštitu informacija</span><span class="sxs-lookup"><span data-stu-id="0eaea-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="0eaea-116">Pregled dokumentacije za zaštitu od Azure informacija</span><span class="sxs-lookup"><span data-stu-id="0eaea-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="0eaea-117">Zahtevi za zaštitu od Azure informacija</span><span class="sxs-lookup"><span data-stu-id="0eaea-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="0eaea-118">Brzo pokretanje obuka za Azure zaštitu informacija</span><span class="sxs-lookup"><span data-stu-id="0eaea-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="0eaea-119">Preuzimanje programa za zaštitu od Azure informacija</span><span class="sxs-lookup"><span data-stu-id="0eaea-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)