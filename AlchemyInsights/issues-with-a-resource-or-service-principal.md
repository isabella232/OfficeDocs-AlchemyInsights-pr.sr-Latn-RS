---
title: Problemi sa resursom resursa ili usluge
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714084"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemi sa resursom resursa ili usluge

1. Ako ste samo prvi koraci, [aplikacije i glavne objekte u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) opisuju registraciju aplikacija, objekte aplikacije i direktorove usluge u usluzi Azure Active Directory: Šta je to, kako se koriste i kako su povezani međusobno. Scenarij koji sadrži i više stanara takođe se prikazuje kako bi ilustrovao relaciju između objekta aplikacije aplikacije i odgovarajućih objekata osnovnih usluga.
2. Više o relaciji između aplikacija i glavnih usluga možete da saznate tako što ćete pročitati [aplikacije i glavne objekte u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Kako da: koristite portal za kreiranje AZURE oglašavanja i direktora usluge koji mogu da pristupe resursima](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) prikazuje kako da kreirate novi Azure Active Directory (AZURE AD) aplikacija i direktor usluge koji se može koristiti sa kontrolom pristupa na osnovu uloge.
4. Uz [glavni API usluge](https://docs.microsoft.com/graph/api/resources/serviceprincipal)možete da upravljate instancama aplikacija i kontrolišete šta aplikacija može da uradi u vašem zakupcu.
5. [tip resursni tip resursa](https://docs.microsoft.com/graph/api/resources/serviceprincipal) navodi sva svojstva i metode za tip resursa serviceglavni resurs.
6. [Razlike tipa resursa između AZURE AD grafika i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) ističu razlike između Azure AD grafgrafa i Microsoft Graph resursa. Prikazuje resurse koji imaju različita imena ili nisu dostupni; takođe naglašava resurse dostupne u beta verziji programa Microsoft Graph, ali ne u programu v 1.0.

**Problemi sa korisnicima gostiju**

- [Brzi Start: dodajte korisnike gosta u direktorijum na Azure portalu](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) vam pokazuje kako da dodate novog gosta korisnika u vaš Azure direktorijum oglasa preko Azure portala, pošaljete pozivnicu i vidite kako izgleda proces iskupljenja korisnika gosta.
- [Uputstvo: Kreiranje korisničkih tokova u usluzi Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) prikazuje kako da kreirate neke preporučene korisnike tokova pomoću Azure portala. Ako tražite informacije o tome kako da podesite protok lozinki korisnika resursa (ROPC) u aplikaciji, pogledajte članak konfigurisanje akreditiva lozinki vlasniku resursa u Azure AD B2C.
