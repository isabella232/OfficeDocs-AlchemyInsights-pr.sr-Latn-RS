---
title: Problemi sa uslovnim pristupom
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069978"
---
# <a name="conditional-access-issues"></a>Problemi sa uslovnim pristupom

**Rešavanje problema sa dijagnostičkim prijavljivanjem**

Pomoću dijagnostike za prijavljivanje možete brzo da saznate šta se dogodilo ili da ustanovite probleme u vezi sa prijavljivanjem [korisnika:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Pokrenite dijagnostiku za prijavljivanje.
1. Pronađite događaj za analiziranje tako što ćete uneti detalje koje imate o korisniku, aplikaciji, vremenu prijave, ID-u zahteva ili ID-u korelacije.
1. Pregledajte dijagnostički rezultate koji pokazuju detalje o tome šta se dogodilo i koje radnje možete preduzeti da biste promenili (ako su potrebne neke promene).

**Koraci za rešavanje problema sa prijavljivanjem** 

1. Prešli na stranicu za prijavljivanje u Azure AD.
1. Filtriranje prijava po korisniku, vremenskom opsegu, aplikaciji, statusu, klijentnoj aplikaciji i tako dalje.
1. Izaberite događaj prijava i prikažite karticu Uslovni pristup da biste videli koje smernice su procenjene.
1. Kliknite na red smernica da biste prikazali detalje smernica i razumeli zašto je primenjena.

**Alatke za rešavanje problema sa smernicama uslovnog pristupa**

- Režim samo za izveštaje vam omogućava da procenite smernice bez uticaja na korisnike.
- Alatka "Šta-ako" vam je dozvolila da simulirate događaje za prijavljivanje i vidite koje smernice se primenjuju.
- Uvidi i izveštavanja o radnoj svesci prikazuju uticaj svake smernice u realnom vremenu.

**Smernice za zaštitu osnovnih linija**

Smernice za zaštitu osnovnih linija su uklonjene. One se više ne nagomilaju i uskoro će biti uklonjene sa Azure portala. Preporučujemo da omogućavate [podrazumevane vrednosti bezbednosti.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Dodatne informacije o uslovnom pristupu potražite u:

[Najbolje prakse za uslovni pristup u programu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrole u uslovnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokacije u uslovnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
