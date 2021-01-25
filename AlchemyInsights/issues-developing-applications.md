---
title: Problemi pri razvoju aplikacija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974769"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="607c6-102">Problemi pri razvoju aplikacija</span><span class="sxs-lookup"><span data-stu-id="607c6-102">Issues developing applications</span></span>

<span data-ttu-id="607c6-103">Da biste rešili uobičajene probleme prilikom pravljenja Azure Active Directory (AD) aplikacija, pogledajte sledeće članke:</span><span class="sxs-lookup"><span data-stu-id="607c6-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="607c6-104">Vidim problem sa prijavljivanjem u aplikacije pomoću samo pregledača</span><span class="sxs-lookup"><span data-stu-id="607c6-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="607c6-105">Ne znam kako da promenim podrazumevane vrednosti trajanja simbola za moju aplikaciju</span><span class="sxs-lookup"><span data-stu-id="607c6-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="607c6-106">Zbunjena/o tome kako funkcioniše pristanak aplikacije</span><span class="sxs-lookup"><span data-stu-id="607c6-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="607c6-107">Ne znam kako da odobrim dozvole za aplikaciju</span><span class="sxs-lookup"><span data-stu-id="607c6-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="607c6-108">Ne razumem razliku između dozvola "delegirana i aplikacija"</span><span class="sxs-lookup"><span data-stu-id="607c6-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="607c6-109">\***Kraj podrške za Azure Active Directory potvrda identiteta biblioteke (ADALE) i AZURE AD Graph Graf (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="607c6-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="607c6-110">Počevši od 30 juna, 2020, više nećemo dodavati nijednu novu funkciju u biblioteku Azure aktivnog direktorijuma (ADALA) i API Azure AD Graph (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="607c6-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="607c6-111">Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.</span><span class="sxs-lookup"><span data-stu-id="607c6-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="607c6-112">Počevši od 30 juna, 2022, okončavamo podršku za ADALA i AAD Graf i više neće pružiti tehničku podršku ili bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="607c6-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="607c6-113">Kao rezultat ovog uslova, slede implikacije:</span><span class="sxs-lookup"><span data-stu-id="607c6-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="607c6-114">Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće dobiti tehničku podršku ili bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="607c6-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="607c6-115">Aplikacije koje koriste AAD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke AAD Graph</span><span class="sxs-lookup"><span data-stu-id="607c6-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="607c6-116">/*Adala migracija*\*</span><span class="sxs-lookup"><span data-stu-id="607c6-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="607c6-117">Ako koristite Microsoft aplikacije, preporučujemo da ažurirate u Microsoft biblioteci autentifikacije (MSAL), koja ima najnovije funkcije i bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="607c6-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="607c6-118">Ova preporuka je u kontekstu programa Microsoft da inicira proces migriranja njegovih aplikacija na MSAL po krajnjim rokovima.</span><span class="sxs-lookup"><span data-stu-id="607c6-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="607c6-119">Migracija za Microsoft aplikacije na MSAL obezbeđuje da aplikacije imaju korist od tekuće bezbednosti i poboljšanja funkcija.</span><span class="sxs-lookup"><span data-stu-id="607c6-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="607c6-120">Pročitajte ADNO najčešća pitanja</span><span class="sxs-lookup"><span data-stu-id="607c6-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="607c6-121">Saznajte kako da migrirate aplikacije na osnovu osnove po platformi</span><span class="sxs-lookup"><span data-stu-id="607c6-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="607c6-122">Ako vam je potrebna pomoć u razumevanju koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i, ako je primenljivo, da pristupite bilo kom nezavisnom dobavljaču proizvoda (ISVs) ili dobavljačima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="607c6-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="607c6-123">Microsoft podrška vam takođe može pružiti listu svih aplikacija koje ne podržavaju Microsoft u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="607c6-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="607c6-124">**AAD Graph migracija**</span><span class="sxs-lookup"><span data-stu-id="607c6-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="607c6-125">Za aplikacije koje koriste AAD Graph potražite uputstvo za migraciju AAD dijagrama u Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="607c6-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="607c6-126">[Naša kontrolna lista za migraciju pruža taиku na početku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="607c6-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="607c6-127">Vaš Azure registracioni portal pokazuje koje aplikacije koriste AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="607c6-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="607c6-128">Preporučujemo da pregledate sve izvorne kodove za aplikacije i da, ako je primenljivo, pristupite bilo kom nezavisnom dobavljaču proizvoda (ISVs) ili dobavljačima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="607c6-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="607c6-129">Microsoft podrška vam pruža i informacije o korišćenju AAD dijagrama u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="607c6-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







