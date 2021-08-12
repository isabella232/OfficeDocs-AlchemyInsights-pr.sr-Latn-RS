---
title: Oznake osetljivosti se ne pojavljuju
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
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061446"
---
# <a name="sensitivity-labels-not-appearing"></a>Oznake osetljivosti se ne pojavljuju

Oznake osetljivosti vam omogućavaju da klasifikujte i zaštitite osetljiv sadržaj. Oni mogu da se kreiraju u Microsoft 365 centar za usaglašenost, Microsoft 365 centru za bezbednost ili Microsoft 365 centru za bezbednost & za usaglašenost u okviru oznake > klasifikacije > osetljivosti. Da biste saznali više o ovoj funkciji, [pogledajte pregled oznaka osetljivosti.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Ako ste konfigurisali oznake osetljivosti, ali se one ne pojavljuju u Microsoft 365 aplikacijama, proverite sledeće:

- Potvrdite da je oznaka osetljivosti [objavljena](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) za korisnike i grupe koje želite.

- Potvrdite da korisnik koristi aplikaciju koja podržava oznake osetljivosti – pogledajte oznake osetljivosti [u dokumentu.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Ako migrirate [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)oznake, imajte na umu stvari navedene [ovde.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Podrška za sprečavanje gubitka podataka (DLP: Trenutno, samo oznake zadržavanja mogu da se koriste kao uslov u DLP smernicama.  Podrška za oznake osetljivosti u DLP smernicama još nije dostupna, ali radimo na tome.

- Kada je šifrovanje omogućeno na oznaci osetljivosti, možete da odaberete da:
    - Dodelite dozvole odmah
    - Omogućavanje korisnicima da dodele dozvole


Za više informacija o mogućim problemima pogledajte [Poznati problemi sa oznakama osetljivosti.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)