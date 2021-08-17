---
title: Napravite e-poruku koja se hvata sve
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
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080760"
---
# <a name="create-an-email-catch-all"></a>Napravite e-poruku koja se hvata sve

Upotreba zahladanja je veoma odsutan. Bolje je da obezbedite odskok pošiljaocu i tako ga pustite da zna da nije moguće isporučiti poruku kako bi mogli da preduzme radnju. Takođe možete da ograničite nadgledano poštansko sanduče tako da prima samo ranije važeće e-adrese. 

Svako hvatanje svakog poštanskog sandučeta dobiće dobru ponudu bezb. I na kraju ih može popuniti ako se ne nadgleda pažljivo. (Postoje ograničenja za prijem.) 

Ako odlučite da nastavite, pratite ove korake:

1. Kreiranje dinamičke grupe za distribuciju & "Svi tipovi primalaca".

2. Kreirajte namenski poštansko sanduče da biste hvatali e-poruke, na primer catchall@domain.com.

3. Za određeni domen podesite DomainType na "InternalRelay". Ako kasnije uklonite sve stavke, uverite se da ste domen vratili na "Ovlašćeno".

4. Kreirajte pravilo za prenos toka pošte na sledeći način:

    - Ako pošiljalac ima "Izvan organizacije"
    - Preusmerite poruku na Catchall@domain.com
    - Osim ako je primalac član grupe allusers@domain.com (grupa za distribuciju sadrži sve članove)
    - Proverite da li je provera valjanosti novih poštanskih sandučića dodata u dinamičkoj grupi za distribuciju
