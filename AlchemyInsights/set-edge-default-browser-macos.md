---
title: Podešavanje pregledača Microsoft Edge kao podrazumevanog pregledača na macOS uređaju
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491813"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="6853b-102">Podešavanje pregledača Microsoft Edge kao podrazumevanog pregledača na macOS uređaju</span><span class="sxs-lookup"><span data-stu-id="6853b-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="6853b-103">Koristite jedan od ova dva metoda da biste postavili Microsoft Edge kao podrazumevani pregledač:</span><span class="sxs-lookup"><span data-stu-id="6853b-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="6853b-104">1. metod: Bljesnite uređaj pomoću slike macOS-a gde je Microsoft Edge već podešen kao podrazumevani pregledač.</span><span class="sxs-lookup"><span data-stu-id="6853b-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="6853b-105">2. metod: Podesite smernice DefaultBrowserSettingEnabled da biste od korisnika tražili da postavi Microsoft Edge kao podrazumevani pregledač.</span><span class="sxs-lookup"><span data-stu-id="6853b-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="6853b-106">Oba metoda omogućavaju korisniku da promeni podrazumevani pregledač.</span><span class="sxs-lookup"><span data-stu-id="6853b-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="6853b-107">Iz tog razloga, preporučujemo da primenite smernicu DefaultBrowserSettingEnabled čak i ako ste koristili metod 1.</span><span class="sxs-lookup"><span data-stu-id="6853b-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="6853b-108">Ako korisnik promeni podrazumevani pregledač nakon primene smernica, smernice će zatražiti od korisnika da podrazumevani pregledač vrati na Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="6853b-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
