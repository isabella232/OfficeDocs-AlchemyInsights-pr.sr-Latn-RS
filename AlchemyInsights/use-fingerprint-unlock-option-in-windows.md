---
title: Koristite opciju otključanog otiska prsta u Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971949"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Koristite opciju otključanog otiska prsta u Windows 10

**Omogućavanje Windows Hello otisaka prstiju**

Da biste otključali Windows 10 pomoću otiska prsta Windows Hello, morate da podesite otisak prsta tako što ćete dodati (kako Windows da nauči da prepozna) najmanje jednim prstom. 

1. Idite na **Postavke > Nalozi > za prijavljivanje** (ili kliknite [ovde](ms-settings:signinoptions?activationSource=GetHelp)). Navodi se dostupne opcije za prijavljivanje. Na primer:

    ![Opcije za prijavljivanje.](media/sign-in-options.png)

2. Izaberite ili **dodirnite Windows Hello stavku Otisak prsta**, a zatim **izaberite stavku Podešavanje**. U prozoru Windows Hello podešavanje izaberite stavku **Prvi koraci.** Senzor za otisak prsta će se aktivirati i od vas će se tražiti da stavite prst na senzor:

   ![Senzor otisaka prstiju.](media/fingerprint-sensor.png)

3. Sledite uputstva koja će zatražiti od vas da više puta skenirate prst. Kada ovo završite, imaćete opciju da dodate druge prste koje ćete možda želeti da koristite za prijavljivanje. Sledeći put kada se prijavite Windows 10, imaćete opciju da koristite otisak prsta da to uradite.

**Windows Hello Otisak prsta nije dostupan kao opcija za prijavljivanje**

Ako Windows Hello otisak prsta nije prikazan kao opcija u opcijama za **prijavljivanje,** to znači da Windows ne zna za čitač otisaka prstiju/skener povezan sa računarom ili da sistemske smernice sprečavaju njegovu upotrebu (ako, na primer, vašim računarom upravlja radno mesto). Da biste rešili problem: 

1. Kliknite na **dugme Start** na traci zadataka i potražite stavku **Upravljač uređajima.**

2. Izaberite ili dodirnite da biste **otvorili Upravljač uređajima.**

3. U upravljaču uređajima razvijte biometrijske uređaje tako što ćete kliknuti na ševron.

   ![Biometrički uređaji.](media/biometric-devices.png)

4. Skener otisaka prstiju treba da bude naveden kao biometrički uređaj, kao što je Synaptics WBDI skener:

   ![Biometrički uređaji.](media/biometric-devices-expanded.png)

5. Ako skener otisaka prstiju nije prikazan, a skener je integrisan u računar, idite na veb sajt proizvođača računara. U odeljku za tehničku podršku za model računara potražite upravljački Windows 10 za skener koji možete da instalirate.

6. Ako je skener odvojen od računara (povezan putem USB),idite na veb sajt proizvođača skenera da biste pronašli i instalirali Windows 10 softver upravljačkog programa uređaja za model skenera koji imate.
