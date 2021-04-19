---
title: Nije moguće pristupiti SharePoint ili OneDrive centru aktivnosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824449"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Nije moguće pristupiti SharePoint ili OneDrive centru aktivnosti

- Ako je lokacija SharePoint ili OneDrive centra administratora nedostupna ili je nedostupna, možda postoji privremeni problem sa uslugom gde korisnici nailaziju na povremena odlaganja ili greške u navigaciji prilikom pristupa SharePoint lokacijama ili OneDrive sadržaju. Proverite [kontrolnu tablu Za zdravstveno stanje usluge](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste videli da li to utiče na vašu organizaciju.

- Globalnim i SharePointadministartima treba dodeliti SharePoint licencu. Novi kreirani nalozi koji su upravo dodeljeni sa ulogom SharePoint licence ili ulogom administarcionog može imati problema sa pristupom programu SharePoint, kao što su "pristup je odbijen" ili "nije pronađen korisnik". Sačekajte najmanje 24 časa da se sinhronizacija dovrši u svim sistemima. Razumemo da 24 časa mogu izgledati kao dugo vreme. U mnogim slučajevima već radimo na rešenju.

- Korisnici privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) mogu da dobiju pristup odbijen ako je veoma mali prozor vremena dozvoljenog pristupa. Pogledajte pristup zabranjen [PIM nalozima.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)