---
title: Konfigurisanje postavki privatnosti u programu Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405734"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="9f608-102">Konfigurisanje postavki privatnosti u programu Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="9f608-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="9f608-103">Ako je Microsoft Edge primenen na platformama koje nisu Windows, dijagnostički podaci i informacije o lokaciji ne šalju se korporaciji Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9f608-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="9f608-104">Međutim, ako se Microsoft Edge koristi u operativnom sistemu Windows 10, dijagnostički podaci i informacije o lokaciji se šalju u skladu sa postavkama Windows dijagnostičkih [podataka korisnika.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="9f608-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="9f608-105">Da biste konfigurisali način na koji Microsoft Edge rukuje kolekcijom podataka za organizaciju, koristite sledeće smernice grupe:</span><span class="sxs-lookup"><span data-stu-id="9f608-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="9f608-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) uključuje izveštavanje o korišćenjem i podacima koji se odnose na padove.</span><span class="sxs-lookup"><span data-stu-id="9f608-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="9f608-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) šalje informacije o lokaciji koje se koriste za poboljšanje Microsoft usluga.</span><span class="sxs-lookup"><span data-stu-id="9f608-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="9f608-108">Da biste saznali više, pogledajte [konfigurisanje postavki smernica.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="9f608-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
