---
title: Problemi u razvoju aplikacija
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013438"
---
# <a name="issues-developing-applications"></a>Problemi u razvoju aplikacija

Da biste rešili najčešće probleme prilikom Azure Active Directory aplikacije (AD), pogledajte sledeće članke:

- [Naišla sam na problem sa prijavljivanjem u aplikacije samo pomoću pregledača Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Ne znam kako da promenim podrazumevane vrednosti tokena za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Zbunjuje me način na koji funkcioniše pristanak na aplikaciju](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Ne znam kako da dodelim dozvole za aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Ne razumem razliku između delegirane i dozvole za aplikacije](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Kraj podrške za Azure Active Directory biblioteke potvrde identiteta (ADAL) i Azure AD Graph API (AAD Graph)***

- Od 30. juna 2020. više nećemo dodavati nove funkcije u Azure Active Directory Authentication Library (ADAL) i Azure AD Graph API (AAD Graph). Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.

- Od 30. juna 2022. prestaćemo sa podrškom za ADAL i AAD Graph i više nećemo pružati tehničku podršku ili bezbednosne ispravke. Kao rezultat ovog uslova, ovo su implikacije:

    - Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da rade i nakon ovog vremena, ali neće dobiti nikakvu tehničku podršku ili bezbednosne ispravke.

    - Aplikacije koje koriste AAD Graph nakon ovog vremena možda više neće primati odgovore iz AAD Graph krajnje tačke

**ADAL migracija**

Ako koristite Microsoft aplikacije, preporučujemo da ga ažurirate na Microsoft Authentication Library (MSAL), koja sadrži najnovije funkcije i bezbednosne ispravke. Ova preporuka je u kontekstu korporacije Microsoft koja pokreće proces migracije aplikacija u MSAL do kraja roka podrške. 

Migracija od strane korporacije Microsoft u MSAL obezbeđuje pogodnosti aplikacija od trenutnih poboljšanja bezbednosti i funkcija usluge MSAL.

1. [Pročitajte najčešća pitanja za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Saznajte više o tome kako da migrirate aplikacije na osnovu platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste ADAL, preporučujemo da pregledate izvorni kôd svih aplikacija i da se, ako je primenljivo, ćaskate svim nezavisnim dobavljačima softvera (ISV-ovima) ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste AAD Graph, pratite naša uputstva da biste migrirali AAD Graph aplikacije u Microsoft Graph:

1. [Naša lista za migraciju pruža tačku za početak](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate izvorni kôd svih aplikacija i, ako je to primenljivo, do nezavisnih dobavljača softvera (ISV-ove) ili dobavljača aplikacija. Microsoft podrška takođe može da vam pruži informacije o AAD Graph o tome kako se koristi u vašem zakuatoru.







