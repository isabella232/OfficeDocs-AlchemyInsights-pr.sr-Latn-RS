---
title: Postavke pokretanja u aplikaciji Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909840"
---
# <a name="startup-settings-in-windows-10"></a>Postavke pokretanja u aplikaciji Windows 10

**Promena aplikacija koje se pokrećaju automatski pri pokretanju**

1. Idite na [Postavke > Aplikacije > pokretanje](ms-settings:startupapps?activationSource=GetHelp).

2. Uverite se da je uključena bilo koja aplikacija koju želite da pokrenete pri **pokretanju.**

**Dodavanje aplikacije koja će se automatski pokrenuti pri pokretanju**

1. Kliknite na dugme **Start ili je** dodirnite i pronađite aplikaciju koju želite da pokrenete pri pokretanju.

2. Kliknite desnim tasterom miša na aplikaciju, izaberite **stavku Još**, a zatim **izaberite stavku Otvori lokaciju datoteke**. To otvara lokaciju na kojoj je sačuvana prečica do aplikacije. Ako ne postoji opcija za Otvaranje lokacije datoteke, to znači da aplikacija ne može da se pokrene pri pokretanju.

3. Kada je lokacija datoteke otvorena, pritisnite taster **sa Windows sa logotipom + R,** otkucajte **shell:pokretanje**, a zatim kliknite na dugme **U redu.** To otvara fasciklu "Pokretanje".

4. Kopirajte i nalepite prečicu do aplikacije sa lokacije datoteke u pokrenu fasciklu.

**Napredne opcije za pokretanje (uključujući Sef režima rada, UEFI postavke i pokretanje sa drugog uređaja)**

1. Sačuvajte rad i zatvorite sve otvorene dokumente jer će ovi koraci ponovo pokrenuti računar.

2. Idite na Postavke > [Ažuriranje & bezbednosti > oporavak.](ms-settings:recovery?activationSource=GetHelp)

3. U **okviru Napredno pokretanje izaberite** stavku **Ponovo pokreni odmah.** 

4. Kada se računar ponovo pokrene na ekran Izbor opcije:

    - Da biste se pokrećeli sa uređaja kao što je USB disk, **izaberite stavku Koristi uređaj**.

    - Da biste uneli UEFI postavke (ponekad se naziva BIOS instalacija), izaberite stavku Rešavanje problema > napredne opcije > **UEFI firmver Postavke.** 

    - Da biste Sef u režim pokretanja ili promenili napredne postavke pokretanja, izaberite stavku **Rešavanje problema >** napredne opcije > pri pokretanju Postavke izaberite stavku Ponovo pokreni.  Možda će vam biti zatraženo da [unesete BitLocker ključ za oporavak.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Kada se računar ponovo pokrene, kliknite na postavku pokretanja koji želite da koristite.