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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405334"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>Tajna klijenta za registraciju aplikacije ili problemi sa certifikatom

Tajni klijent aplikacije koji je u toku?

Bez obzira na to kako je napravljena registrovana aplikacija, bilo putem standardnog procesa registracije na portalu za registraciju aplikacija ili ako je principal usluge kreiran u zakucaku pomoću pristanka aplikacije, nova tajna klijenta mora da se kreira pre isteka trenutnog i ažurira se u povezanom kodu aplikacije. Maksimalni period važenja je 2 godine. Kao podsetnik, tajna vrednost mora da se snimi jer više neće biti vidljiva kada napustite stranicu registracije aplikacija na portalu. Više informacija potražite u članku Brzi start: Registrovanje aplikacije na [platformi Microsoft identiteta](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) i Najbolje prakse za [platformu Microsoft identiteta.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Da biste saznali više, pogledajte [članak Kreiranje Azure AD aplikacije & principal usluge na portalu – platforma Microsoft identitet.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
