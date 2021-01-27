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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015001"
---
# <a name="conditional-access-issues"></a>Problemi sa uslovnim pristupom

**Rešavanje problema sa dijagnostičkim rešenjem**

Možete brzo da saznate šta se dešava ili pronađu probleme u vezi sa prijavljivanjem korisnika pomoću [dijagnostike za prijavljivanje](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Pokrenite dijagnostiku prijavljivanja.
1. Pronađite događaj koji treba analizirati tako što ćete uneti detalje koje imate o korisniku, aplikaciji, vremenu prijavljivanja, ID-u zahteva ili ID korelacije.
1. Pregledajte rezultate dijagnoze koji prikazuju detalje šta se dogodilo i koje radnje možete preduzeti da biste izvršili promene (ako su potrebne promene).

**Koraci za rešavanje problema sa prijavljivanjem** 

1. Idite na stranicu za prijavljivanje na Azure AD.
1. Prijavljivanje na filtriranje pomoću korisnika, vremenske vrednosti, zatvaranja, statusa, aplikacije klijenta itd.
1. Izaberite događaj prijavljivanja i prikažite karticu uslovno pristup da biste videli koje smernice se procenjuju.
1. Kliknite na redu smernica da biste prikazali detalje o politici i razumeli zašto se to odnosi.

**Alatke za rešavanje problema sa uslovnim pristupom**

- Režim samo za izveštavanje omogućava vam da procenite smernice bez zaostalih korisnika.
- Alatka "Šta-ako" vam omogućava da simulirate događaje prijavljivanja i vidite koje se smernice primenjuju.
- Radna sveska sa shvatanju i prijavljivanju prikazuje uticaj svake smernice u realnom vremenu.

**Smernice za zaštitu osnovnih linija**

Smernice za zaštitu osnovnih linija su neodobrene. Više se ne primenjuju i uskoro će biti uklonjene iz Azure portala. Preporučujemo omogućavanje [postavki bezbednosti](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Više informacija o uslovnom pristupu potražite u članku:

[Najbolje prakse za uslovno pristup u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Uslovi u uslovnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Kontrole u uslovnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Lokacije u uslovnom pristupu](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
