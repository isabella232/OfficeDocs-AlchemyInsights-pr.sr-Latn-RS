---
title: Evidencija lozinki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527180"
---
# <a name="password-logs"></a>Evidencija lozinki

**Imam problema sa pristupanjem evidenciji nadzora za poništavanje lozinke**

Da biste rešili probleme u vezi sa pristupom za pristup evidenciji nadzora, uradite sledeće:

Obezbedite da imate ovlašćenje za prikaz evidencija nadzora. 

Odobrene su samo sledeće uloge:
 - Globalni administrator
 - Administrator bezbednosti
 - Čitač bezbednosti

**Želim da vidim sve događaje nadgledanja poništene iz vremena koje sam prvobitno rasporedila**

Do 120.000 resetovanja lozinki/prijava se skladište u izveštajima prethodnih 30 dana. Ovo ograničenje se odnosi na UI kada preuzmete CSV. 1.000.000 događaji su dostupni kroz PowerShell.
Dodatne informacije potražite u članku dolenavedene veze:

- [Samouslužni događaji poništavaju događaje iz Azure AD izveštaja i API događaja](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Kako da brzo preuzmete događaje registracije lozinki pomoću PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Želim da razumem više o mogućnostima izveštavanja o poništavanju lozinke**

Potvrdite ko se registruje za ili uspostavlja početnu vrednost lozinki pomoću usluge Azure AD password poništi evidentiranja nadzora na Azure sajtu u okviru **korisnici i grupe**.
Više informacija potražite u sledećim vezama:

- [Pregled izveštaja o poništavanju lozinke](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Kako se prikazuju izveštaji o poništavanju lozinke na Azure portalu](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Samouslužni događaji poništavaju događaje iz Azure AD izveštaja i API događaja](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Kako da brzo preuzmete događaje registracije lozinki pomoću PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


