---
title: Tajna klijenta za registraciju aplikacije ili problemi sa certifikatom
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
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951507"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Tajna klijenta za registraciju aplikacije ili problemi sa certifikatom

Tajni klijent aplikacije koji je u toku?

Bez obzira na to kako je napravljena registrovana aplikacija, bilo putem standardnog procesa registracije na portalu za registraciju aplikacija ili ako je principal usluge kreiran u zakucaku pomoću pristanka aplikacije, nova tajna klijenta mora da se kreira pre isteka trenutnog i ažurira se u povezanom kodu aplikacije. Maksimalni period važenja je 2 godine. Kao podsetnik, tajna vrednost mora da se snimi jer više neće biti vidljiva kada napustite stranicu registracije aplikacija na portalu. Više informacija potražite u brzom [startu: Registrovanje](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) aplikacije u Microsoft platforma za identitete [i Najbolje prakse za Microsoft platforma za identitete.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Da biste saznali više, [pogledajte kreiranje Azure AD aplikacije & principal usluge na portalu – Microsoft platforma za identitete.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
