---
title: Izbriši zakuca
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993907"
---
# <a name="delete-tenant"></a>Izbriši zakuca

Da biste izbrisali Azure AD, uverite se da:
- Vi ste globalni administrator u direktorijumu.
- Niste prijavljeni sa nalogom koji ima podrazumevani direktorijum kao što je contoso.onmicrosoft.com na potpisanom nalogu – na primer, admin@contoso.onmicrosoft.com.
- Uklonite sve aktivne aplikacije u direktorijumu pre brisanja. Da biste uklonili aktivne aplikacije, pomerite se do registracija aplikacija i uklonite postojeće aplikacije.
- Nema aktivnih pretplata za nijednu Microsoft Online Services uslugu, kao što su Microsoft Azure, Office 365 ili Azure AD Premium povezane sa direktorijumom. Prenesete pretplate ili ubrzate otkazivanje aktivnih pretplata putem Azure podrške i naplate. Saznajte više o tome Kako da otkažete Office 365 i Azure pretplate. Uputstva o povezivanju ili dodavanju postojeće pretplate u zakupca možete da povežete ili dodate Azure pretplatu u [Azure AD zakupca.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Nema aktivne licence. Da biste uklonili licence, pogledajte [kako da uklonite pretplatu za uklanjanje licence.](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)
- Nema drugih aktivnih korisnika u direktorijumu osim vas kao globalnog administratora kada pokušavate da izbrišete Azure AD. Uklonite sve druge aktivne korisnike, a sve zavisnosti od prilagođenog imena domena u zakupca takođe treba da se uklone, kao što su korisnici kreirani admin@contoso.com.

Detaljnije korake o tome kako da:
- Ako izbrišete Azure Active Directory" ili "pretplatu", pogledajte brisanje [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Uklanjanje aplikacija u direktorijumu, pogledajte [uklanjanje aplikacija.](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app) 
