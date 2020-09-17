---
title: Nije moguće izbrisati stavke u sistemu SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806125"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e9052-102">Nije moguće izbrisati stavke</span><span class="sxs-lookup"><span data-stu-id="e9052-102">Unable to delete items</span></span>

<span data-ttu-id="e9052-103">Smernice za zadržavanje mogu uzrokovati ovu grešku, treba da onemogućite ili isključite odgovarajući čekanje koji uzrokuje ovaj problem.</span><span class="sxs-lookup"><span data-stu-id="e9052-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="e9052-104">Kada se ukloni polisa za zadržavanje ili čekanje, može biti potrebno do 24 časa da bi promena stupila na snagu.</span><span class="sxs-lookup"><span data-stu-id="e9052-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="e9052-105">Uverite se da nije podešena [smernica za zadržavanje](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) za stavku.</span><span class="sxs-lookup"><span data-stu-id="e9052-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="e9052-106">Lokacija je možda premašila ograničenje skladišta, povećavanje [kvote](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i brisanje stavke.</span><span class="sxs-lookup"><span data-stu-id="e9052-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="e9052-107">Uverite se da stavka nije [odjavljena](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) na drugog korisnika.</span><span class="sxs-lookup"><span data-stu-id="e9052-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="e9052-108">Konačno, administratori mogu da koriste [SharePoint obrasce i prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) koji sadrže biblioteku PowerShell komandi koje vam omogućava da obavljate komplikovane radnje upravljanja kao što je prinudno brisanje tvrdoglavih stavki.</span><span class="sxs-lookup"><span data-stu-id="e9052-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="e9052-109">Ukloni PNP datoteku</span><span class="sxs-lookup"><span data-stu-id="e9052-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e9052-110">Uklanjanje PNP fascikle</span><span class="sxs-lookup"><span data-stu-id="e9052-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e9052-111">Uklanjanje stavke PNP liste</span><span class="sxs-lookup"><span data-stu-id="e9052-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e9052-112">Ukloni PNP listu</span><span class="sxs-lookup"><span data-stu-id="e9052-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e9052-113">Uklanjanje PNP polja (kolona)</span><span class="sxs-lookup"><span data-stu-id="e9052-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)