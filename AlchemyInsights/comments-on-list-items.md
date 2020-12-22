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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724168"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="b898f-102">Komentari na listi stavki</span><span class="sxs-lookup"><span data-stu-id="b898f-102">Comments on List items</span></span>

<span data-ttu-id="b898f-103">Korisnici mogu da pregledaju sve komentare na stavci liste i da filtriraju između prikaza koji prikazuju komentare ili aktivnosti povezane sa stavkom.</span><span class="sxs-lookup"><span data-stu-id="b898f-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="b898f-104">Korisnici treba da zabeležite sledeće pre nego što dodaju i brišu komentare:</span><span class="sxs-lookup"><span data-stu-id="b898f-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="b898f-105">Komentari slede postavke dozvola koje su svojstvene u sistemu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b898f-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="b898f-106">Klasične liste koje još uvek nisu ugrađene da se pojave u modernim korisničkim interfejsima, kao što su liste zadataka, neće imati ovu funkciju komentarišanje.</span><span class="sxs-lookup"><span data-stu-id="b898f-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="b898f-107">Komentarišanje listi u timovima nije dostupno ovim izdanjima.</span><span class="sxs-lookup"><span data-stu-id="b898f-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="b898f-108">Pretraživanje komentara nije Indeksirano.</span><span class="sxs-lookup"><span data-stu-id="b898f-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="b898f-109">Administratori mogu da onemoguće ovu funkciju na nivou organizacije tako što ćete promeniti parametar " **pohvalkalistitemsonemogućavanje** "  u PowerShell cmdlet usluzi.</span><span class="sxs-lookup"><span data-stu-id="b898f-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="b898f-110">Trenutno nije moguće onemogućiti komentarisanje na lokaciji ili nivou liste.</span><span class="sxs-lookup"><span data-stu-id="b898f-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="b898f-111">Nadamo se da ćemo imati te kontrole u kasnijoj ispravci, verovatno u prvom kvartalu 2021.</span><span class="sxs-lookup"><span data-stu-id="b898f-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
