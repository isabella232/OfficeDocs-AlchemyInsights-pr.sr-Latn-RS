---
title: Kreiranje e-poruke
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713000"
---
# <a name="create-an-email-catch-all"></a>Kreiranje e-poruke

Upotreba hvatanja je odlučno obeshrabrena. Bolje je da se ponovo vratite na pošiljalac koji omogućava pošiljaoce da saznaju da poruka nije mogla da se dostavi kao adresirana kako bi mogla da preduzme radnju. Praćenom poštanskom sandučetu možete da ograničite samo da biste imali važeće e-adrese. 

Bilo koji ulov sve poštansko sanduče dobiće dobar deo bezvredne pošte i može na kraju popuniti ako se pažljivo ne nadgleda. (Postoje ograničenja za primanje.) 

Ako odlučite da nastavite, pratite ove korake:

1. Kreirajte dinamičku grupu za distribuciju & uključujete "sve tipove primalaca".

2. Kreiranje namenskog poštanskog sandučeta za hvatanje e-poruka, na primer, catchall@domain.com.

3. Za određeni domen, postavljanje domena za domen "Inter". Ako kasnije uklonite sve hvatanje, obavezno ponovo konfigurišete domen za autoritativno.

4. Kreirajte pravilo transporta Pošilka na sledeći način:

    - Ako je pošiljalac "izvan organizacije"
    - Preusmeravanje poruke na Catchall@domain.com
    - Osim ako je primalac član allusers@domain.com (grupna raspodela sadrži sve članove)
    - Uverite se da su novi poštanski sandučići dodati u grupu za dinamiku distribucije
