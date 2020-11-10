---
title: Komentari na listi stavki
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
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982559"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="dce70-102">Komentari na listi stavki</span><span class="sxs-lookup"><span data-stu-id="dce70-102">Comments on List items</span></span>

<span data-ttu-id="dce70-103">Korisnici će uskoro moći da dodaju i brišu komentare na stavkama liste.</span><span class="sxs-lookup"><span data-stu-id="dce70-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="dce70-104">Korisnici mogu da pregledaju sve komentare na stavci liste i da filtriraju između prikaza koji prikazuju komentare ili aktivnosti povezane sa stavkom.</span><span class="sxs-lookup"><span data-stu-id="dce70-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="dce70-105">**Tajming** :</span><span class="sxs-lookup"><span data-stu-id="dce70-105">**Timing** :</span></span>

<span data-ttu-id="dce70-106">**Ciljano izdanje** : postepeno se vrti sredinom oktobra i očekuje se da će biti završen do sredine novembra</span><span class="sxs-lookup"><span data-stu-id="dce70-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="dce70-107">**Standardno izdanje** : postepeno se vrti u sredinom novembra i očekuje se da će biti završen početkom decembra</span><span class="sxs-lookup"><span data-stu-id="dce70-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="dce70-108">**Rollout** Prijem: ciljano izdanje za celu organizaciju</span><span class="sxs-lookup"><span data-stu-id="dce70-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="dce70-109">Korisnici treba da zabeležite sledeće pre nego što dodaju i brišu komentare:</span><span class="sxs-lookup"><span data-stu-id="dce70-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="dce70-110">Komentari slede postavke dozvola koje su svojstvene u sistemu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dce70-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="dce70-111">Klasične liste koje još uvek nisu ugrađene da se pojave u modernim korisničkim interfejsima, kao što su liste zadataka, neće imati ovu funkciju komentarišanje.</span><span class="sxs-lookup"><span data-stu-id="dce70-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="dce70-112">Komentarišanje listi u timovima nije dostupno ovim izdanjima.</span><span class="sxs-lookup"><span data-stu-id="dce70-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="dce70-113">Pretraživanje komentara nije Indeksirano.</span><span class="sxs-lookup"><span data-stu-id="dce70-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="dce70-114">Administratori mogu da onemoguće ovu funkciju na nivou organizacije tako što ćete promeniti parametar " **pohvalkalistitemsonemogućavanje** " **Set-SPOTenant** u PowerShell cmdlet usluzi.</span><span class="sxs-lookup"><span data-stu-id="dce70-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="dce70-115">Trenutno nije moguće onemogućiti komentarisanje na lokaciji ili nivou liste.</span><span class="sxs-lookup"><span data-stu-id="dce70-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="dce70-116">Nadamo se da ćemo imati te kontrole u kasnijoj ispravci, verovatno u prvom kvartalu 2021.</span><span class="sxs-lookup"><span data-stu-id="dce70-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
