---
title: Rešavanje problema sa savršenim prijavljivanjem zasnovanim na lozinkama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714885"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Rešavanje problema sa savršenim prijavljivanjem zasnovanim na lozinkama

Da biste naučili osnove SSO lozinki, pogledajte članak [potvrda identiteta zasnovanu na lozinci sa uslugom Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfigurisanje SSO-a zasnovan na lozinci**

1. [Konfigurisanje jedinstvenog prijavljivanja na zasnovan na lozinci](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -ovaj članak sadrži detaljnije informacije o opciji SSO na osnovu lozinke. Ako aplikacija koju dodajete zahteva prilagođenu konfiguraciju i morate da koristite SSO na osnovu lozinki, ovaj članak je za vas.
2. [Konfigurisanje jedinstvenog prijavljivanja na zasnovan na lozinci za aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) " Prijavljivanje zasnovano na lozinci je namenjeno aplikacijama koje koriste kombinaciju korisničkog imena/lozinki za potvrdu identiteta. Kada konfigurišete prijavljivanje na osnovu lozinki za aplikaciju, korisnici moraju da se prijave u lokalnu aplikaciju jednom. Posle toga, Azure Active Directory skladišti informacije za prijavljivanje i automatski je pruža aplikaciji kada korisnici pristupe daljinski.
    - Trebalo je da objavite i testirate aplikaciju sa proxy serverom. Ako to ne uradite, slijedite korake u odeljku [objavljivanje aplikacija pomoću usluge Azure AD Application proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)

Da biste rešili problem sa lozinkom zasnovanim na lozinci, pogledajte članak [Rešavanje problema sa jedinstvenim prijavljivanjem zasnovanim na lozinci](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
