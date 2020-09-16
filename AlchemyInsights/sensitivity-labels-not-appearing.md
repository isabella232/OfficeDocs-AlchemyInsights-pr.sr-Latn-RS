---
title: Oznake osećajnosti ne prikazuju se
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801198"
---
# <a name="sensitivity-labels-not-appearing"></a>Oznake osećajnosti ne prikazuju se

Oznake poverljivosti vam omogućava da klasifikujete i zaštitite osetljiv sadržaj. One mogu da se kreiraju u Microsoft 365 centru za usaglašenost, Microsoft 365 Security Center ili Microsoft 365 Security & centar za usaglašenost u okviru oznake poverljivosti >. Da biste saznali više o ovoj funkciji, pogledajte članak [Pregled oznaka osećajnosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Ako ste konfigurisali oznake osećajnosti, ali se ne pojavljuju u Microsoft 365 aplikacijama, potvrdite sledeće:

- Potvrdite da je oznaka poverljivosti [objavljena](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) za korisnike i grupe koje želite.

- Potvrdite da korisnik koristi aplikaciju koja podržava oznake osećajnosti – pogledajte [oznake osećajnosti u dokumentu](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Ako [migriram usluge Azure zaštite informacija](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), imajte na [umu navedene informacije](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Podrška za sprečavanje gubitka podataka (DLP): trenutno se samo nalepnice za zadržavanje mogu koristiti kao uslov u programu DLP.  Podrška za oznake osećajnosti u programu DLP još uvek nije dostupna, ali radimo na tome.

- Kada je šifrovanje omogućena na nalepnici poverljivosti, možete da odaberete sledeće:
    - Odmah dodeli dozvole
    - Omogućite korisnicima da dodele dozvole


Više informacija o mogućim problemima potražite u članku [poznati problemi sa oznakama osećajnosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).