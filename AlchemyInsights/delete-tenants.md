---
title: Brisanje zakupca
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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564882"
---
# <a name="delete-tenant"></a>Brisanje zakupca

Da biste izbrisali Azure reklamu, obezbedite:
- Vi ste globalni administrator u direktorijumu.
- Niste prijavljeni pomoću naloga koji ima podrazumevani direktorijum kao što je contoso.onmicrosoft.com na nalogu, kao što je admin@contoso.onmicrosoft.com.
- Uklonite sve aktivne aplikacije u direktorijumu pre brisanja. Da biste uklonili aktivne aplikacije, pređite na registraciju aplikacija i uklonite postojeće aplikacije.
- Ne postoje aktivne pretplate za bilo koje Microsoft usluge na mreži, kao što je Microsoft Azure, Office 365 ili Azure AD Premium povezane u direktorijumu. Prebacite pretplate ili ubrzano otkazivanje aktivnih pretplata putem Azure podrške i naplate. Saznajte više o tome kako da otkažete Office 365 i Azure pretplate. Za uputstva o asocijaciji ili dodavanju postojeće pretplate zakupcu pogledajte [članak pridruživanje Azure usluzi AZURE AD zakupcu](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Nema aktivne licence. Da biste uklonili licence, pogledajte [Kako da uklonite pretplatu da biste uklonili licencu](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Ne postoje drugi aktivni korisnici u direktorijumu osim kada pokušate da izbrišete Azure AD. Uklonite sve aktivne korisnike i bilo koje zavisnosti od prilagođenog imena domena u zakupcu i treba da se uklone, kao što su korisnici kreirani admin@contoso.com.

Dodatne detalje o tome kako da:
- Izbrišite "Azure Active Directory" ili "pretplata", pogledajte članak [Brisanje Azure aktivnog direktorijuma](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Uklanjanje aplikacija iz direktorijuma potražite u članku [Uklanjanje aplikacija](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
