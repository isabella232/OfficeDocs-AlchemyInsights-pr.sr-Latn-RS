---
title: Postavke pokretanja u operativnom sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751149"
---
# <a name="startup-settings-in-windows-10"></a>Postavke pokretanja u operativnom sistemu Windows 10

**Promena aplikacija automatski se pokreće prilikom pokretanja**

1. Idite na [postavke > aplikacije > pokretanju](ms-settings:startupapps?activationSource=GetHelp).

2. Proverite da li **je uključena aplikacija**koju želite da pokrećete prilikom pokretanja.

**Dodavanje aplikacije za automatsku pokretanje prilikom pokretanja**

1. Kliknite ili dodirnite stavku **Započni** i pronađite aplikaciju koju želite da pokrenete prilikom pokretanja.

2. Kliknite desnim tasterom miša na aplikaciju, kliknite na dugme **još**, a zatim izaberite stavku **Otvori lokaciju datoteke**. Tako ćete otvoriti lokaciju na kojoj se čuva prečica do aplikacije. Ako ne postoji opcija za lokaciju za otvaranje datoteke, to znači da aplikacija ne može da se pokrene prilikom pokretanja.

3. Ako je lokacija datoteke otvorena, pritisnite taster sa **Windows logotipom + R**, otkucajte **Shell: pokretanje**, a zatim kliknite na dugme **u redu**. Ovo otvara fasciklu za pokretanje.

4. Kopirajte i nalepite prečicu na aplikaciju sa lokacije datoteke u polaznoj fascikli.

**Napredne opcije pokretanja (uključujući bezbedni režim, UEFI postavke i pokretanje sa drugog uređaja)**

1. Sačuvajte posao i zatvorite sve otvorene dokumente, pošto će ovi koraci ponovo pokrenuti računar.

2. Idite na [postavke > ažurirajte & bezbednost > oporavku](ms-settings:recovery?activationSource=GetHelp).

3. U okviru **Više opcija za pokretanje**kliknite na dugme **Ponovo pokreni odmah**. 

4. Kada se računar ponovo pokrene na stranici izbor opcije:

    - Da biste pokrenuli pokretanje sa uređaja kao što je USB disk, kliknite na dugme **koristi uređaj**.

    - Da biste uneli postavke UEFI (koje se ponekad nazivaju podešavanje BIOS-a), izaberite stavku **Rešavanje problema > napredne opcije > UEFI firmware postavke**. 

    - Da biste uneli bezbedni režim ili promenili napredne postavke pokretanja, izaberite stavku **rešavanje > više opcija > postavkama pokretanja**, a zatim izaberite stavku **Ponovo pokreni**. Od vas će biti zatraženo da unesete [BitLocker ključ za oporavak](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Kada se računar ponovo pokrene, izaberite postavku za pokretanje koju želite da koristite.