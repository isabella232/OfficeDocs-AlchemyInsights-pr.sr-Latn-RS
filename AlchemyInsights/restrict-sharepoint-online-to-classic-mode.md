---
title: Ograničavanje sistema SharePoint Online na klasični režim
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751436"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="f1d52-102">Ograničavanje sistema SharePoint Online na klasični režim</span><span class="sxs-lookup"><span data-stu-id="f1d52-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="f1d52-103">Neke organizacije i dalje zahtevaju iskustvo klasičnog režima.</span><span class="sxs-lookup"><span data-stu-id="f1d52-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="f1d52-104">Iako ne postoje planovi za uklanjanje klasičnog režima na zrnasti nivo, više nije moguće ograničiti celu organizaciju (stanar) u klasični režim za liste i biblioteke.</span><span class="sxs-lookup"><span data-stu-id="f1d52-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="f1d52-105">Administrator će imati sledeće opcije za upravljanje pojedinačnim listama i bibliotekama u klasičnom režimu pomoću prekidača za odbijanje saglasnosti koje pružamo na sledećim nivoima:</span><span class="sxs-lookup"><span data-stu-id="f1d52-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="f1d52-106">kolekcija lokacija</span><span class="sxs-lookup"><span data-stu-id="f1d52-106">site collection</span></span>
- <span data-ttu-id="f1d52-107">stranica</span><span class="sxs-lookup"><span data-stu-id="f1d52-107">site</span></span>
- <span data-ttu-id="f1d52-108">list</span><span class="sxs-lookup"><span data-stu-id="f1d52-108">list</span></span>
- <span data-ttu-id="f1d52-109">njoj</span><span class="sxs-lookup"><span data-stu-id="f1d52-109">library</span></span>

<span data-ttu-id="f1d52-110">Pored toga, liste koje koriste određene funkcije i prilagođavanja koje savremeni ne podržavaju, i dalje će se automatski prebaciti na klasični režim.</span><span class="sxs-lookup"><span data-stu-id="f1d52-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="f1d52-111">Počevši od 1 do aprila 2019, proces onemogućavanja nivoa zakupca na nivou savremene liste i biblioteka počeće i nastavlja 2019 se kroz 31.</span><span class="sxs-lookup"><span data-stu-id="f1d52-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="f1d52-112">Liste i biblioteke koji su u klasičnom režimu kao rezultat umanjeni pristup zakupcu automatski će biti pomereni na moderno.</span><span class="sxs-lookup"><span data-stu-id="f1d52-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="f1d52-113">Ako vam je potreban klasični režim, pogledajte članak više informacija [ovde](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) i PNP PowerShell uputstvo [ovde](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) koji opisuje opcije i alatke koje možete da koristite danas da biste koristili iskustvo klasičnog režima.</span><span class="sxs-lookup"><span data-stu-id="f1d52-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
