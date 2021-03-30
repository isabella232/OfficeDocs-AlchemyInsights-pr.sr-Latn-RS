---
title: Aplikacija za potvrdu identiteta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405679"
---
# <a name="authentication-app"></a>Aplikacija za potvrdu identiteta

Ako ste globalni administ, možete brzo da saznate šta se dogodilo ili da ustanovite probleme povezane sa korisničkim prijavljivanjem pomoću funkcije "Dijagnostika [za prijavljivanje"](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. Pokrenite dijagnostiku tako što ćete kliknuti na dugme["Pokreni dijagnostiku".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Pronađite događaj za analiziranje tako što ćete uneti detalje koje imate o korisniku, aplikaciji, vremenu prijave, ID-u zahteva ili ID-u korelacije.
1. Pregledajte dijagnostički rezultate koji pokazuju detalje o tome šta se dogodilo i koje radnje možete preduzeti da biste promenili po potrebi.

**Proverite da li je scenario primenljiv:**

1. Ako korisnik ne dobija push obaveštenje u aplikaciji Microsoft Authenticator, potvrdite da se korisnici ne prikazuju u okviru MFA blokiranih korisnika kao što je opisano u članku Blokiranje i [deblokiranje korisnika.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Ako korisnik nije blokiran za MFA, ali ne primi push obaveštenje, može da otvori aplikaciju Microsoft Authenticator, koja povlači zahteve za odobrenje na čekanju.
1. Kao alternativni metod prijave, korisnik može i da klikne na "Prijavite se na drugi način" i odabere da koristi kôd za verifikaciju iz moje aplikacije za mobilne uređaje.
1. Aplikacija Microsoft Authenticator je jedini dostupan metod za veliki broj korisnika. [Saznajte više o podrazumevanim vrednostima bezbednosti](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), najčešća pitanja o aplikaciji [Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) za najčešća pitanja i kako da ih rešite.
 
**Preporučeni video zapisi**

[Kako da podesite aplikaciju Authenticator na novom telefonu (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
