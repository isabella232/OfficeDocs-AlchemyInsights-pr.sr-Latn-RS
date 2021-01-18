---
title: Konfiguracija proxy aplikacije
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885526"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="3fd24-102">Konfiguracija proxy aplikacije</span><span class="sxs-lookup"><span data-stu-id="3fd24-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="3fd24-103">Da biste razumeli kako da konfigurišete aplikaciju proxy servera u okviru Azure AD da biste izložili lokalne aplikacije u oblaku, pogledajte [članak konfigurisanje proxy aplikacije za aplikaciju](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="3fd24-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="3fd24-104">Jedinstveno prijavljivanje (SSO) omogućava korisnicima da pristupe aplikaciji bez autentične identiteta.</span><span class="sxs-lookup"><span data-stu-id="3fd24-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="3fd24-105">Omogućava jedinstvenu potvrdu identiteta koja se pojavljuje u oblaku, protiv Azure aktivnog direktorijuma i omogućava uslugu ili konektor da oponaša korisnika da bi dovršio sve dodatne izazove potvrde identiteta iz aplikacije.</span><span class="sxs-lookup"><span data-stu-id="3fd24-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="3fd24-106">Da biste saznali više, pogledajte [članak konfigurisanje jedinstvenog prijavljivanja u proxy aplikaciji aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="3fd24-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="3fd24-107">Koristite [Ovaj članak](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) da biste rešili probleme sa uobičajenim problemima koje osobe suočavaju kada kreiraju novu proxy aplikaciju aplikacije.</span><span class="sxs-lookup"><span data-stu-id="3fd24-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="3fd24-108">Ako imate problem sa podešavanjem potvrde identiteta na svoju aplikaciju, možda će biti potrebno da [rešite probleme Kerberos konfiguracije delegiranja u delegaciji aplikacije](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ili da biste sledili uputstva za [Konfigurisanje aplikacije sa pingbonom](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) da biste rešili problem.</span><span class="sxs-lookup"><span data-stu-id="3fd24-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
