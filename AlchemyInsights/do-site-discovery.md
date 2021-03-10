---
title: Otkrivanje lokacija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694559"
---
# <a name="do-site-discovery"></a><span data-ttu-id="3b2d3-102">Otkrivanje lokacija</span><span class="sxs-lookup"><span data-stu-id="3b2d3-102">Do site discovery</span></span>

<span data-ttu-id="3b2d3-103">Ako organizacija i dalje koristi zastarele Veb aplikacije i planove za korišćenje programa Internet Explorer (koje većina klijenata ima), trebalo bi da uradite nešto dodatno otkrivanje lokacije.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="3b2d3-104">**Već ste rasporedili stariju verziju Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="3b2d3-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="3b2d3-105">Ako ste već konfigurisali listu preduzeća da radi za nasleđenu verziju sistema Microsoft Edge, otkrivanje lokacije će biti gotovo gotovo.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="3b2d3-106">Jedina stvar koju treba da uradite je da dodate neutralne lokacije.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="3b2d3-107">Neutralne lokacije najčešće su lokacije koje pružaju jedinstveno prijavljivanje (SSO).</span><span class="sxs-lookup"><span data-stu-id="3b2d3-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="3b2d3-108">Ako odete na neutralnu lokaciju sa lokacije Microsoft Edge, želite da ostanete u aplikaciji Microsoft Edge da biste se potvrdili autentičnosti.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="3b2d3-109">Ako odete na neutralnu stranicu u režimu programa Internet Explorer, zatim želite da ostanete u režimu programa Internet Explorer da biste potvrdili autentičnost.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="3b2d3-110">Identifikujte SSO ili druge neutralne lokacije koje koristite i dodajte ih na listu poslovnih lokacija.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="3b2d3-111">**Internet Explorer je podrazumevani pregledač**</span><span class="sxs-lookup"><span data-stu-id="3b2d3-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="3b2d3-112">Ako sada koristite samo Internet Explorer, možda ne znate koje su lokacije nadograđene na moderne Veb standarde i koje i dalje zahtevaju Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="3b2d3-113">Ove lokacije ćete želeti da pronađete i dodate na listu lokacije preduzeća kako biste mogli da koristite Internet Explorer samo za te lokacije.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="3b2d3-114">[Otkrivanje lokacije preduzeća](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) otkriva lokacije kojima je možda potreban Internet Explorer režim.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="3b2d3-115">Možete prikupiti podatke na računarima koji rade pod operativnim sistemom Windows Internet Explorer 8 putem Internet Explorer 11 u operativnom sistemu Windows 10, Windows 8,1 ili Windows 7.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="3b2d3-116">**Analiza podataka**</span><span class="sxs-lookup"><span data-stu-id="3b2d3-116">**Analyze the data**</span></span>

<span data-ttu-id="3b2d3-117">Pošto ste prikupili podatke na sajtu, preporučujemo da sledeći proces iz četiri koraka analizira podatke:</span><span class="sxs-lookup"><span data-stu-id="3b2d3-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="3b2d3-118">Sortirajte podatke po domenu, a zatim po URL adresi.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="3b2d3-119">Definišite granice aplikacije za konfiguraciju za Internet Explorer režim.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="3b2d3-120">Želite da dodate sve lokacije i Veb kontrole koje definišu aplikaciju, ali ne želite da dodate dodatne lokacije i kontrole.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="3b2d3-121">Neke lokacije mogu biti jednostavne kao i *https://contoso.com/app1* dok će drugi možda zahtevati da definišete više sajtova i stranica.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="3b2d3-122">Testirate aplikaciju da biste proverili da li izvorno radi.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="3b2d3-123">Mnoge lokacije će ponuditi moderan sadržaj kada otkriju moderni pregledač i ponude zastareli sadržaj samo kada otkriju Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="3b2d3-124">Dodajte aplikaciju na listu poslovnih lokacija ako ne uspe da testira.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="3b2d3-125">Kao najbolju praksu, grupišete sve lokacije koje sačinjavaju aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="3b2d3-126">Na ovaj način, kada nadogradite aplikaciju, možete lakše da uklonite celu stranicu iz režima programa Internet Explorer i počnete da koristite moderan pregledač za tu aplikaciju.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="3b2d3-127">Kada završite sa otkrivanjem sajta i analizirajte podatke, spremni ste da počnete da tražite strategiju kanala.</span><span class="sxs-lookup"><span data-stu-id="3b2d3-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

