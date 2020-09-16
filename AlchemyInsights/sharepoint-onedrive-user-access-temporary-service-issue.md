---
title: Problemi sa performansama – SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771258"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="9a68d-102">SharePoint ili OneDrive spori, nedostupni ili nedostupni za više korisnika</span><span class="sxs-lookup"><span data-stu-id="9a68d-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="9a68d-103">Ako OneDrive ili SharePoint lokacija nisu dostupni većem broju korisnika koji su prethodno imali Access, možda postoji privremeno izdanje.</span><span class="sxs-lookup"><span data-stu-id="9a68d-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="9a68d-104">[Potvrdite izbor u polju za zdravstvenu zaštitu usluge](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="9a68d-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="9a68d-105">**Dodavanje i licenciranje korisnika**</span><span class="sxs-lookup"><span data-stu-id="9a68d-105">**Add and license the user**</span></span>

<span data-ttu-id="9a68d-106">Uverite se da ste [korisnicima dodelili licence u usluzi Microsoft 365 za preduzeća](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="9a68d-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="9a68d-107">**Dodeljivanje dozvola**</span><span class="sxs-lookup"><span data-stu-id="9a68d-107">**Assign Permissions**</span></span>

<span data-ttu-id="9a68d-108">Ako je korisniku dodeljena SharePoint licenca i još uvek prima pristup odbijen pristup, uverite se da je dodeljen [odgovarajući nivo dozvole](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="9a68d-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="9a68d-109">**Razmotrite korišćenje funkcije Access zahteva**</span><span class="sxs-lookup"><span data-stu-id="9a68d-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="9a68d-110">[Funkcija Access zahteva](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućava osobama da zahtevaju pristup sadržaju koji trenutno nemaju dozvolu da vide.</span><span class="sxs-lookup"><span data-stu-id="9a68d-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="9a68d-111">**Dozvolite prilagođenoj skriptama može dovesti do problema sa zabranom pristupa**</span><span class="sxs-lookup"><span data-stu-id="9a68d-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="9a68d-112">Postoje određeni scenariji gde funkcija " *Dozvolite prilagođenu* poruku" može da predstavlja pristup koji je zabranjen.</span><span class="sxs-lookup"><span data-stu-id="9a68d-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="9a68d-113">Za listu pogođene funkcije, bezbednosna pitanja i mogućnost onemogućavanja funkcije.</span><span class="sxs-lookup"><span data-stu-id="9a68d-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="9a68d-114">Posetite [stavku Omogući ili sprečite prilagođenu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)poruku.</span><span class="sxs-lookup"><span data-stu-id="9a68d-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

