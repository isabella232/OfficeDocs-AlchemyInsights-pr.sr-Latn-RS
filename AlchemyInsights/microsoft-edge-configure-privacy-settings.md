---
title: Microsoft Edge Konfigurisanje postavki privatnosti
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
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678858"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="57bf4-102">Microsoft Edge Konfigurisanje postavki privatnosti</span><span class="sxs-lookup"><span data-stu-id="57bf4-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="57bf4-103">Ako se Microsoft Edge raspoređena na platformama koje nisu Windows, dijagnostičke podatke i informacije o lokaciji se ne šalju korporaciji Microsoft.</span><span class="sxs-lookup"><span data-stu-id="57bf4-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="57bf4-104">Međutim, ako je Microsoft Edge primenjen u operativnom sistemu Windows 10, informacije o dijagnostici i lokaciji se šalju u skladu sa korisničkim [postavkama podataka Windows dijagnostika](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="57bf4-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="57bf4-105">Da biste konfigurisali kako Microsoft Edge obrađuje prikupljanje podataka za organizaciju, koristite sledeće smernice grupe:</span><span class="sxs-lookup"><span data-stu-id="57bf4-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="57bf4-106">[Metricsreportingen](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Ova smernica omogućava izveštavanje o korišćenju i podacima o padu.</span><span class="sxs-lookup"><span data-stu-id="57bf4-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="57bf4-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Ova smernica šalje informacije o lokaciji koje se koriste za poboljšanje Microsoft usluga.</span><span class="sxs-lookup"><span data-stu-id="57bf4-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="57bf4-108">Da biste saznali više, pogledajte članak [Konfigurisanje postavki smernica](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="57bf4-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>