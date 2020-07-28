---
title: Nije moguće promeniti korisničko ime
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440300"
---
# <a name="unable-to-change-username"></a>Nije moguće promeniti korisničko ime

U nekim slučajevima, UPN (UserPrincipalName) promene nisu razdeljene u oblaku. Možete da primite greške pri proveri valjanosti na Office 365 portalu ili da ne možete da promenite korisničko ime ili e-adresu. Da biste rešili ovaj problem, ručno podesite UserPrincipalName koristeći ovu komandu "PowerShell".

**Primer: preimenovanje korisnika**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName-Korisnikprincipalname "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

Ova komanda preimenuje davidc@contoso.com na davidchew@contoso.com.

Više informacija potražite u članku [Postavljanje-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).