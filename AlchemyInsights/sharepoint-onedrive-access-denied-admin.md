---
title: Rešavanje problema sa pristupom "zabranjen pristup"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707968"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="3c294-102">Rešavanje problema sa pristupom zabranjen poruka u sistemu SharePoint/OneDrive centar administracije</span><span class="sxs-lookup"><span data-stu-id="3c294-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="3c294-103">Ako dobijate poruku o zabranjeni pristup prilikom pokušaja da posetite SharePoint/OneDrive centar administracije, uverite se da ste [korisniku dodelili licencu](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="3c294-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="3c294-104">Ako korisnik ima licencu, trebalo bi da se uverite da su im [dodeljene uloge administratora](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) koje mogu da pristupe administratorskim centrima.</span><span class="sxs-lookup"><span data-stu-id="3c294-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="3c294-105">Ovaj problem takođe može da se pojavi kada se korisnik izbriše i ponovo kreira sa istim direktorom glavnog imena (UPN).</span><span class="sxs-lookup"><span data-stu-id="3c294-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3c294-106">Novi nalog se kreira pomoću različitog korisničkog polja (Passport unikatni ID).</span><span class="sxs-lookup"><span data-stu-id="3c294-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3c294-107">Kada korisnik pokuša da pristupi kolekciji lokacija ili svom OneDrive, korisnik ima neispravni PUID.</span><span class="sxs-lookup"><span data-stu-id="3c294-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3c294-108">Drugi scenario uključuje sinhronizaciju direktorijuma sa organizacionim jedinicama aktivnog direktorijuma (OU).</span><span class="sxs-lookup"><span data-stu-id="3c294-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3c294-109">Ako su se korisnici već prijavili u sistemu SharePoint, a zatim se premeštaju u drugačiji a i ponovo sinhronizuju sa sistemom SharePoint, oni mogu da doћive ovaj problem.</span><span class="sxs-lookup"><span data-stu-id="3c294-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="3c294-110">Da biste rešili ovaj problem, trebalo bi da vratite originalni UPN sa koracima u članku, [vratite korisnika u prethodno stanje u usluzi Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="3c294-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="3c294-111">Napomena: ako OneDrive ili SharePoint centar administracije nisu dostupni većem broju korisnika koji su prethodno imali Access, možda postoji privremeno izdanje.</span><span class="sxs-lookup"><span data-stu-id="3c294-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="3c294-112">[Potvrdite izbor u polju za zdravstvenu zaštitu usluge](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="3c294-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


