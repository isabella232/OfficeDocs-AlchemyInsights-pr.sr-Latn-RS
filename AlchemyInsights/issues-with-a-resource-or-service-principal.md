---
title: Problemi sa resursom ili principalom usluge
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028090"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemi sa resursom ili principalom usluge

1. Ako tek počinjete sa radom, objekti aplikacije i usluge u programu Azure Active Directory opisuju registraciju, objekte aplikacije i principale usluga u programu Azure Active Directory: šta su, kako se koriste i kako su [međusobno](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) povezani. Ujedno je predstavljen i scenario sa više zakupaca za ilustrovanje odnosa između objekta aplikacije aplikacije i odgovarajućih glavnih objekata usluge.
2. Možete da saznate više o relacijama između aplikacija i principala usluga tako što ćete pročitati aplikacije i glavne objekte usluge u [programu Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. Kako da: Koristite portal da biste kreirali [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) aplikaciju i principal usluge koja može da pristupi resursima pokazuje kako da kreirate novu Azure Active Directory (Azure AD) aplikaciju i principal usluge koja može da se koristi uz kontrolu pristupa zasnovanu na ulozi.
4. Uz principal [usluge API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)možete programski da upravljate instancama aplikacija i da kontrolišete šta aplikacija može da radi u okviru zakupca.
5. [servicePrincipal tip resursa](https://docs.microsoft.com/graph/api/resources/serviceprincipal) navodi sva svojstva i metode za servicePrincipal tip resursa.
6. Razlike u tipu resursa između [Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) ističe razlike između Azure AD Graph i Microsoft Graph resursa. Prikazuje resurse koji imaju različita imena ili nisu dostupni; takođe ističe resurse dostupne u beta verziji korporacije Microsoft Graph ali ne i u verziji v1.0.

**Problemi sa korisnicima sa u goste**

- Brzi start: Dodavanje korisnika sa u goste u direktorijum na [Azure portalu](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) pokazuje kako da dodate novog korisnika sa u goste u Azure AD direktorijum putem Azure portala, pošaljete pozivnicu i vidite kako izgleda proces eskanja poziva korisnika sa pozivima za gosta.
- Uputstvo: Kreiranje tokova korisnika u [programu Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) pokazuje kako da kreirate neke preporučene tokove korisnika pomoću Azure portala. Ako tražite informacije o tome kako da podesite tok akreditiva vlasnika resursa (ROPC) u aplikaciji, pogledajte tkup akreditiva vlasnika resursa u Azure AD B2C.
