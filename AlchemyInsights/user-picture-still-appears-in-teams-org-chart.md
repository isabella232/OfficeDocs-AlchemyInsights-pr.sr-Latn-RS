---
title: Slika korisnika se i dalje pojavljuje u Microsoft Teams organizacionim grafikonom
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422320"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Slika korisnika se i dalje pojavljuje u Microsoft Teams organizacionim grafikonom

Ako je onemogućeno ili uklonjeno više pojedinaca iz organizacije, a njihova fotografija profila se i dalje pojavljuje u organizacionom grafikonu, moguće je da je postavka **ShowInAddressLists** postavljena na False: 

1. Idite na Microsoft 365 centar administracije > [aktivni korisnici](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) i izaberite korisnika sa fotografijom koja se i dalje pojavljuje. 
1. Izaberite karticu **Pošta** i uverite se da je opcija **Prikaži na globalnom spisku adresa postavljena** na **Ne**.

Ako podešavanje **stavke ShowInAddressLists** na **"Ne"** ne funkcioniše, proverite sledeće: 

- Korisnik će se možda prikazati sa liste primalaca u Exchange. Dodatne informacije potražite u [članku Upravljanje listama adresa u Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Korisnik se može prikazati sa spiska adresa u e-Azure Active Directory. Više informacija potražite u članku [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 