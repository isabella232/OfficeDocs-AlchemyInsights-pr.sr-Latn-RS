---
title: Microsoft Edge User agent
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
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679335"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="fa250-102">Microsoft Edge User agent</span><span class="sxs-lookup"><span data-stu-id="fa250-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="fa250-103">Niske korisnika agenta (UA) mogu se koristiti za otkrivanje verzije određenog pregledača koja se koristi za određeni operativni sistem.</span><span class="sxs-lookup"><span data-stu-id="fa250-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="fa250-104">Kao i u drugim pregledačima, Microsoft Edge obuhvata ove informacije u HTTP zaglavlju "korisnički agent" svaki put kada zatraži lokaciju.</span><span class="sxs-lookup"><span data-stu-id="fa250-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="fa250-105">Informacijama o pregledaču i verziji možete da pristupite putem JavaScript pomoću upita vrednost "Navigator. Useragentu".</span><span class="sxs-lookup"><span data-stu-id="fa250-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="fa250-106">Preporučujemo da Veb programeri koriste ažuriranje funkcija kada god je to moguće da biste poboljšali održavanje koda, smanjili kôd kvarljivosti i uklonili rizik od raspada koda u slučaju budućih ispravki za UA niske UA.</span><span class="sxs-lookup"><span data-stu-id="fa250-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="fa250-107">Više informacija potražite u članku [Niska korisničkog agensa za Microsoft Edge (radna površina)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span><span class="sxs-lookup"><span data-stu-id="fa250-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>