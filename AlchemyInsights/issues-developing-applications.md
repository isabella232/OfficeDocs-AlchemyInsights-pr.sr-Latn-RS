---
title: Problemi pri razvoju aplikacija
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974769"
---
# <a name="issues-developing-applications"></a>Problemi pri razvoju aplikacija

Da biste rešili uobičajene probleme prilikom pravljenja Azure Active Directory (AD) aplikacija, pogledajte sledeće članke:

- [Vidim problem sa prijavljivanjem u aplikacije pomoću samo pregledača](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ne znam kako da promenim podrazumevane vrednosti trajanja simbola za moju aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Zbunjena/o tome kako funkcioniše pristanak aplikacije](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ne znam kako da odobrim dozvole za aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ne razumem razliku između dozvola "delegirana i aplikacija"](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Kraj podrške za Azure Active Directory potvrda identiteta biblioteke (ADALE) i AZURE AD Graph Graf (AAD Graph)** _

- Počevši od 30 juna, 2020, više nećemo dodavati nijednu novu funkciju u biblioteku Azure aktivnog direktorijuma (ADALA) i API Azure AD Graph (AAD Graph). Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.

- Počevši od 30 juna, 2022, okončavamo podršku za ADALA i AAD Graf i više neće pružiti tehničku podršku ili bezbednosne ispravke. Kao rezultat ovog uslova, slede implikacije:

    - Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće dobiti tehničku podršku ili bezbednosne ispravke.

    - Aplikacije koje koriste AAD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke AAD Graph

/*Adala migracija**

Ako koristite Microsoft aplikacije, preporučujemo da ažurirate u Microsoft biblioteci autentifikacije (MSAL), koja ima najnovije funkcije i bezbednosne ispravke. Ova preporuka je u kontekstu programa Microsoft da inicira proces migriranja njegovih aplikacija na MSAL po krajnjim rokovima. 

Migracija za Microsoft aplikacije na MSAL obezbeđuje da aplikacije imaju korist od tekuće bezbednosti i poboljšanja funkcija.

1. [Pročitajte ADNO najčešća pitanja](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Saznajte kako da migrirate aplikacije na osnovu osnove po platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ako vam je potrebna pomoć u razumevanju koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i, ako je primenljivo, da pristupite bilo kom nezavisnom dobavljaču proizvoda (ISVs) ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje ne podržavaju Microsoft u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste AAD Graph potražite uputstvo za migraciju AAD dijagrama u Microsoft Graph:

1. [Naša kontrolna lista za migraciju pruža taиku na početku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Vaš Azure registracioni portal pokazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate sve izvorne kodove za aplikacije i da, ako je primenljivo, pristupite bilo kom nezavisnom dobavljaču proizvoda (ISVs) ili dobavljačima aplikacija. Microsoft podrška vam pruža i informacije o korišćenju AAD dijagrama u vašem zakupcu.







