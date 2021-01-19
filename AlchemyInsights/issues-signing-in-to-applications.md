---
title: Problemi sa prijavljivanjem u aplikacije
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901327"
---
# <a name="issues-signing-in-to-applications"></a>Problemi sa prijavljivanjem u aplikacije

Da biste otkrili uzrok ili pronašli probleme u vezi sa prijavljivanjem u korisnika, obavite sledeće korake:

1. Pokrenite [dijagnostiku prijavljivanja](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Pronađite događaj za analizu tako što ćete uneti detalje koje imate o korisniku, aplikaciji, vremenu prijavljivanja, ID-u ili ID-u.
3. Pregledajte rezultate dijagnostike koji prikazuju detalje onoga što se dogodilo i radnje koje možete da izvršite da biste izvršili promene ako je potrebno promena.

Slede neki uobičajeni problemi na koje možete da naiđete prilikom prijavljivanja u aplikacije:

1. Vi ili korisnik ste **dovršili prijavljivanje na Azure AD u programu, ali vidite neočekivani odziv** – pogledajte članke [neočekivani pristanak za saglasnost prilikom prijavljivanja na aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) i [neočekivanu grešku prilikom izvršavanja pristanka na aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Vi ili korisnik ste se **direktno prijavili na aplikaciju, ali ne možete da se prijavite na njega iz produpljenaprilagođenog portala ili sa Access panela**: pogledajte [članak rešavanje problema sa prijavljivanjem na aplikaciju iz usluge Azure AD my Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Vi ili korisnik ste **dovršili prijavljivanje na Azure AD, ali aplikacija prikazuje poruku o grešci i ne dozvoljava korisniku da završi tok prijavljivanja**: problem je u tome što aplikacija nije prihvatila odgovor koji je Azure AD izdala. Slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) da biste rešili problem.
4. Vi ili korisnik **ne možete da se prijavite u aplikaciju koja nije u galeriji konfigurisana za jedinstveno prijavljivanje lozinki**: slijedite smernice iz [ovih koraka](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) da biste rešili problem.
5. Vi ili korisnik **ne možete da se prijavite u aplikaciju Azure A.d. galerija konfigurisana za jedinstveno prijavljivanje lozinki**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) da biste rešili problem.
6. Vi ili korisnik **ne možete da se prijavite u Microsoft aplikaciju**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) da biste rešili problem.
7. Vi ili korisnik **ne možete da se prijavite u aplikaciju koja nije u galeriji podešena za jedinstveno prijavljivanje pojedinačno**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) da biste rešili problem.
8. Vi ili korisnik **ne možete da se prijavite u aplikaciju Azure A.d. galerija koja je podešena za federativni pojedinačni prijavljivanje**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) da biste rešili problem.
9. Vi ili korisnik **ne možete da se prijavite u prilagođenu primenu**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) za rešavanje problema.
10. Vi ili korisnik **ne možete da se prijavite u lokalno članstvo pomoću proxy servera Azure AD Application**: slijedite [ove korake](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) da biste rešili problem.

