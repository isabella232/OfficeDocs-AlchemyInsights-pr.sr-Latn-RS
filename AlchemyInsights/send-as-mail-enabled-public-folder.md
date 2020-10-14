---
title: Javna fascikla "Pošalji kao pošta" u EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462072"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="2a0a3-102">Javna fascikla sa omogućenim SendAs poštom</span><span class="sxs-lookup"><span data-stu-id="2a0a3-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="2a0a3-103">Sledeći primer dodeljuje dozvole "Pošalji kao" za javnu fasciklu sa omogućenom uslugom pošte korisniku Jasona.</span><span class="sxs-lookup"><span data-stu-id="2a0a3-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="2a0a3-104">Add-RecipientPermission-identitet ' NewPF1 '-poverenik "Jason"-AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="2a0a3-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="2a0a3-105">Detaljne informacije o sintaksi i parametrima potražite u članku [Dodela dozvola "Pošalji kao" ili "Pošalji u ime" za javne fascikle sa omogućenom poštom](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="2a0a3-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

