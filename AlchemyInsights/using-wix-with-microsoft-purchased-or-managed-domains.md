---
title: Korišćenje Wix veb lokacije uz microsoft kupljene ili kontrolisane domene
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: dd0f8beb8f1871c2c43ac14a7f6d1cce79386fcc353bb2a690ba184904ca5857
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083748"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a>Korišćenje Wix veb lokacije uz microsoft kupljene ili kontrolisane domene

Informacije o tome kako da koristite Wix veb lokaciju sa microsoft kupljenim ili kontrolisanim domenom potražite u članku Ažuriranje DNS zapisa da biste zadržili veb lokaciju kod trenutnog [dobavljača usluge hostinga.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)

Detalje možete da vidite u: 

- Wix članak "Povezivanje domena sa wix mrežom pomoću metoda upućivanja", preporučuje dodavanje DNS zapisa kao što je navedeno u gorenavedenim vezama umesto promene imena servera kada koristite Microsoft 365.

- Ako odaberete da promenite servere imena na Wix, morate da kreirate DNS zapise na lokaciji Wix za Microsoft. Više informacija potražite u članku [Kreiranje DNS zapisa na veb lokaciji Wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).

- Ako je domen kupljen od korporacije Microsoft, nije moguće promeniti servere imena. Ako morate da promenite servere imena, Microsoft kupljen domen mora da se prenese drugom dobavljaču hostinga posle 60 dana. Više informacija potražite u članku [Prenos domena od korporacije Microsoft na drugi host.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
