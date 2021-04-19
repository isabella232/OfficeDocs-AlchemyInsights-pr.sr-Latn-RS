---
title: Omogućavanje ugrađivanje zakasnelih dijaloga za otvaranje izveštaja
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814278"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="66c25-102">Omogućavanje ugrađivanje zakasnelih dijaloga za otvaranje izveštaja</span><span class="sxs-lookup"><span data-stu-id="66c25-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="66c25-103">**Simptom**</span><span class="sxs-lookup"><span data-stu-id="66c25-103">**Symptom**</span></span>

<span data-ttu-id="66c25-104">Korisnici ne mogu da otvore izveštaje.</span><span class="sxs-lookup"><span data-stu-id="66c25-104">Users are unable to open reports.</span></span> <span data-ttu-id="66c25-105">"Nešto nije u redu.</span><span class="sxs-lookup"><span data-stu-id="66c25-105">"Something has gone wrong.</span></span> <span data-ttu-id="66c25-106">Proverite tehničke detalje za više detalja".</span><span class="sxs-lookup"><span data-stu-id="66c25-106">Check technical details for more details."</span></span>

<span data-ttu-id="66c25-107">**Uzrok**</span><span class="sxs-lookup"><span data-stu-id="66c25-107">**Cause**</span></span>

<span data-ttu-id="66c25-108">Izveštaji ne uspevaju da se učitaju u UCI sa greškom "Opis obrasca je bez vrednosti ili nije definisan".</span><span class="sxs-lookup"><span data-stu-id="66c25-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="66c25-109">Izveštaji u UCI i dalje zahtevaju zakasnele dijaloge, tako da sistem klijenta mora da ima omogućeni *allowlegacydialogsembebedding.*</span><span class="sxs-lookup"><span data-stu-id="66c25-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="66c25-110">**Rešenje**</span><span class="sxs-lookup"><span data-stu-id="66c25-110">**Solution**</span></span>

1. <span data-ttu-id="66c25-111">Idite na **karticu Postavke >Administracija > Postavke sistema > Opšte postavke.**</span><span class="sxs-lookup"><span data-stu-id="66c25-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="66c25-112">Postavite opciju "Omogući ugrađivanje određenih zatamnjenih dijaloga u klijentu pregledača "Ujedinjeni interfejs" na **da.**</span><span class="sxs-lookup"><span data-stu-id="66c25-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
