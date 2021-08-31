---
title: Slika korisnika se ne prikazuje u Microsoft Teams organizacionom grafikonu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792884"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Slika korisnika se ne prikazuje u Microsoft Teams organizacionom grafikonu

Ako pojedincima u organizaciji nedostaje fotografija profila u organizacionom grafikonu, moguće je da je postavka **ShowInAddressLists** postavljena na **False:**

1. Idite na Microsoft 365 centar administracije > [**korisnika**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users), a zatim izaberite korisnika sa fotografijom koja nedostaje. 
1. Izaberite karticu **Pošta** i uverite se da je opcija **Prikaži na globalnom spisku adresa postavljena** na **Da.** 

Ako podešavanje **stavke ShowInAddressLists** na **"Da"** ne funkcioniše, proverite sledeće:

- Korisnik je možda skriven sa liste primalaca na listi Exchange. Dodatne informacije potražite u [članku Upravljanje listama adresa u Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Korisnik je možda skriven sa spiska adresa na listi Azure Active Directory. Više informacija potražite u članku [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
