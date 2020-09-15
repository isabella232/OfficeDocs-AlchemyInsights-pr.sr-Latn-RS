---
title: Rešavanje problema sa pristupom usluzi OneDrive for Business sajtovima
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670630"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="3a49d-102">Rešavanje problema sa pristupom usluzi OneDrive for Business sajtovima</span><span class="sxs-lookup"><span data-stu-id="3a49d-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="3a49d-103">Ovaj problem se najčešće javlja kada je korisnik izbrisan i ponovo kreiran sa istim direktorom glavnog imena (UPN).</span><span class="sxs-lookup"><span data-stu-id="3a49d-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="3a49d-104">Novi nalog se kreira pomoću različitog korisničkog polja (Passport unikatni ID).</span><span class="sxs-lookup"><span data-stu-id="3a49d-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="3a49d-105">Kada korisnik pokuša da pristupi kolekciji lokacija ili svom OneDrive, korisnik ima neispravni PUID.</span><span class="sxs-lookup"><span data-stu-id="3a49d-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="3a49d-106">Drugi scenario uključuje sinhronizaciju direktorijuma sa organizacionim jedinicama aktivnog direktorijuma (OU).</span><span class="sxs-lookup"><span data-stu-id="3a49d-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="3a49d-107">Ako su se korisnici već prijavili u sistemu SharePoint, a zatim se premeštaju u drugačiji a i ponovo sinhronizuju sa sistemom SharePoint, oni mogu da doћive ovaj problem.</span><span class="sxs-lookup"><span data-stu-id="3a49d-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="3a49d-108">Da biste rešili ovaj problem, trebalo bi da vratite originalni UPN sa koracima u članku, [vratite korisnika u prethodno stanje u usluzi Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="3a49d-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="3a49d-109">Ako ne možete da vratite originalnog korisnika, trebalo bi da uklonite starog korisnika sa OneDrive lokacije pomoću ovih koraka, [uklonite korisnika sa liste korisničkih informacija]().</span><span class="sxs-lookup"><span data-stu-id="3a49d-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="3a49d-110">Kada to uradite, korisnik može da potvrdi administratorska prava na OneDrive sajtu tako što će pratiti korake za [Dodavanje administratora u OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) .</span><span class="sxs-lookup"><span data-stu-id="3a49d-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="3a49d-111">Više informacija o nivoima dozvola potražite u članku [Razumevanje nivoa dozvola u sistemu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="3a49d-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
