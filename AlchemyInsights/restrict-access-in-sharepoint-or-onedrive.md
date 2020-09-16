---
title: Ograničavanje pristupa u sistemu SharePoint ili OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720696"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="fb8e3-102">Ograničavanje pristupa u sistemu SharePoint ili OneDrive</span><span class="sxs-lookup"><span data-stu-id="fb8e3-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="fb8e3-103">U sistemu SharePoint i OneDrive ograničite pristup stavkama kao što su datoteke, fascikle i liste tako što ćete dodeliti Access samo grupama ili osobama koje želite da imate.</span><span class="sxs-lookup"><span data-stu-id="fb8e3-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="fb8e3-104">Dozvole u sistemu SharePoint podrazumevano su nasleđene iz većeg dodatka u hijerarhiji.</span><span class="sxs-lookup"><span data-stu-id="fb8e3-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="fb8e3-105">Tako da datoteka nasleđuje svoje dozvole iz fascikle, koja nasleđuje dozvole iz biblioteke, koja nasleđuje dozvole od lokacije.</span><span class="sxs-lookup"><span data-stu-id="fb8e3-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="fb8e3-106">Možete da delite na većem nivou (na primer, tako što ćete deliti celu stranicu), a zatim prekinuti nasledstvo ako ne želite da delite sve stavke na lokaciji.</span><span class="sxs-lookup"><span data-stu-id="fb8e3-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="fb8e3-107">Međutim, ovo ne preporučujemo zato što vam ubuduće omogućava da održavate dozvole složenije i zbunjujuće.</span><span class="sxs-lookup"><span data-stu-id="fb8e3-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="fb8e3-108">Evo šta možete da uradite umesto toga:</span><span class="sxs-lookup"><span data-stu-id="fb8e3-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="fb8e3-109">Ako, na primer, želite da delite celokupan sadržaj fascikle, osim za jednu datoteku, premestite tu datoteku na novu lokaciju koja se ne deli.</span><span class="sxs-lookup"><span data-stu-id="fb8e3-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="fb8e3-110">Ako imate dve potfascikle u fascikli i želite da delite jednu potfasciklu sa grupama A i B i omogućite samo pristup grupi u drugu potfasciklu, delite nadređenu fasciklu sa grupom a i dodajte grupu B u prvu potfasciklu.</span><span class="sxs-lookup"><span data-stu-id="fb8e3-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="fb8e3-111">Zaustavljanje deljenja datoteke ili fascikle </span><span class="sxs-lookup"><span data-stu-id="fb8e3-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

