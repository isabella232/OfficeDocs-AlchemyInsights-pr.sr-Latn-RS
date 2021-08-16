---
title: Nije moguće pristupiti SharePoint ili OneDrive centru za administaciju
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
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020458"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Nije moguće pristupiti SharePoint ili OneDrive centru za administaciju

- Ako lokacija SharePoint ili OneDrive centra za administratore nije dostupna ili je nedostupna, možda postoji privremeni problem sa uslugom gde korisnici nailaziju na povremena kašnjenja ili greške u navigaciji prilikom pristupa SharePoint lokacijama ili OneDrive sadržaju. Proverite [kontrolnu tablu Za zdravstveno stanje usluge](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste videli da li to utiče na vašu organizaciju.

- Globalnim i SharePoint treba da se dodelite licenca SharePoint licenci. Novi kreirani nalozi koji su upravo dodeljeni sa ulogom licence ili SharePoint može imati problema sa pristupom programu SharePoint, kao što su "pristup je odbijen" ili "nije pronađen korisnik". Sačekajte najmanje 24 časa da se sinhronizacija dovrši u svim sistemima. Razumemo da 24 časa mogu izgledati kao dugo vreme. U mnogim slučajevima već radimo na rešenju.

- Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) korisnici mogu da dobiju pristup odbijen ako je veoma mali prozor vremena dozvoljenog pristupa. Pogledajte pristup zabranjen [PIM nalozima.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)