---
title: Ograničavanje pristupa u sistemu SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700469"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f0a08-102">Ograničavanje pristupa u sistemu SharePoint ili OneDrive</span><span class="sxs-lookup"><span data-stu-id="f0a08-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f0a08-103">Postoji mnogo načina za ograničavanje pristupa na SharePoint online/OneDrive uslugama.</span><span class="sxs-lookup"><span data-stu-id="f0a08-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="f0a08-104">Ovi različiti metodi ograničenja pristupa su naglašeni ispod.</span><span class="sxs-lookup"><span data-stu-id="f0a08-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="f0a08-105">**Ograničenje dozvole**</span><span class="sxs-lookup"><span data-stu-id="f0a08-105">**Permission Restriction**</span></span>

<span data-ttu-id="f0a08-106">U sistemu SharePoint Online i OneDrive for Business ograničavamo pristup stavkama kao što su lokacije, datoteke i fascikle tako što omogućavamo samo pristup tim grupama/osobama koje treba da imaju pristup.</span><span class="sxs-lookup"><span data-stu-id="f0a08-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="f0a08-107">Prilagođavanje dozvola za SharePoint listu ili biblioteku</span><span class="sxs-lookup"><span data-stu-id="f0a08-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="f0a08-108">Prilagođavanje dozvola za SharePoint sajt</span><span class="sxs-lookup"><span data-stu-id="f0a08-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="f0a08-109">Promena dozvola u potfascikli</span><span class="sxs-lookup"><span data-stu-id="f0a08-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="f0a08-110">Kontrola pristupa iz nekompletnih uređaja</span><span class="sxs-lookup"><span data-stu-id="f0a08-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="f0a08-111">Kao SharePoint ili globalni administrator, možete da blokirate ili ograničite pristup SharePoint i OneDrive sadržaju iz nekompletnih uređaja (oni koji nisu hibridni oglas spojeni u Intune).</span><span class="sxs-lookup"><span data-stu-id="f0a08-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="f0a08-112">**Ograničenje mrežne lokacije**</span><span class="sxs-lookup"><span data-stu-id="f0a08-112">**Network Location Restriction**</span></span>

<span data-ttu-id="f0a08-113">Kao IT administrator, možete da kontrolišete pristup SharePoint i OneDrive resursima na osnovu definisanih mrežnih lokacija u koje imate poverenja.</span><span class="sxs-lookup"><span data-stu-id="f0a08-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="f0a08-114">Ovo je takođe poznato kao smernice zasnovane na lokaciji.</span><span class="sxs-lookup"><span data-stu-id="f0a08-114">This is also known as location-based policy.</span></span> <span data-ttu-id="f0a08-115">Više informacija potražite u članku [Kontrola pristup SharePoint Online i OneDrive podacima na osnovu mrežne lokacije](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="f0a08-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="f0a08-116">**Ograničenje zaključavanje lokacija**</span><span class="sxs-lookup"><span data-stu-id="f0a08-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="f0a08-117">U sistemu SharePoint online imate mogućnost da zaključate kolekciju lokacija, tako da niko nema pristup.</span><span class="sxs-lookup"><span data-stu-id="f0a08-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="f0a08-118">Ovo je podešeno putem programskog dodatka PowerShell i [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću nekretnina [seta-sposite-](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) lockstate.</span><span class="sxs-lookup"><span data-stu-id="f0a08-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="f0a08-119">**Ograničavanje korisnika da kreiraju lokacije ili podlokacije**</span><span class="sxs-lookup"><span data-stu-id="f0a08-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="f0a08-120">Kao SharePoint administrator ili globalni administrator, možete da omogućite korisnicima da kreiraju i upravljaju sopstvenim SharePoint lokacijama, odrede koje lokacije mogu da kreiraju i navode lokaciju lokacija.</span><span class="sxs-lookup"><span data-stu-id="f0a08-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="f0a08-121">Više informacija potražite [u članku Upravljanje kreiranjem lokacije u usluzi SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="f0a08-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

