---
title: Opcija za otključavanje otiska prsta u operativnom sistemu Windows 10
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
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796691"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Opcija za otključavanje otiska prsta u operativnom sistemu Windows 10

**Omogućavanje Windows Hello otiska prsta**

Da biste otključali Windows 10 pomoću otiska prsta, morate da podesite Windows Hello otisak prsta tako što ćete dodati (što će windows učiti da prepozna) najmanje jednim prstom. 

1. Izaberite **stavke Postavke > naloge > za prijavljivanje** (ili kliknite [ovde](ms-settings:signinoptions?activationSource=GetHelp)). Navodi se dostupne opcije za prijavljivanje. Na primer:

    ![Opcije za prijavljivanje.](media/sign-in-options.png)

2. Izaberite ili dodirnite **stavku Windows Hello otisak prsta,** a zatim **izaberite stavku Podešavanje**. U prozoru za konfigurisanje usluge Windows Hello kliknite na **dugme Prvi koraci.** Senzor za otisak prsta će se aktivirati i od vas će se tražiti da stavite prst na senzor:

   ![Senzor otisaka prstiju.](media/fingerprint-sensor.png)

3. Sledite uputstva koja će zatražiti od vas da više puta skenirate prst. Kada ovo završite, imaćete opciju da dodate druge prste koje ćete možda želeti da koristite za prijavljivanje. Sledeći put kada se prijavite u Windows 10, imaćete opciju da koristite otisak prsta da biste to uraditi.

**Windows Hello otisak prsta nije dostupan kao opcija za prijavljivanje**

Ako Windows Hello otisak prsta nije prikazan kao opcija u opcijama za **prijavljivanje,** to znači da Windows ne zna za čitač otisaka prstiju/skener povezan sa računarom ili da sistemske smernice sprečavaju njegovu upotrebu (ako na primer, vašim računarom upravlja vaše radno mesto). Da biste rešili problem: 

1. Kliknite na **dugme Start** na traci zadataka i potražite stavku **Upravljač uređajima.**

2. Izaberite ili dodirnite da biste **otvorili Upravljač uređajima.**

3. U upravljaču uređajima razvijte biometrijske uređaje tako što ćete kliknuti na ševron.

   ![Biometrički uređaji.](media/biometric-devices.png)

4. Skener otisaka prstiju treba da bude naveden kao biometrički uređaj, kao što je Synaptics WBDI skener:

   ![Biometrički uređaji.](media/biometric-devices-expanded.png)

5. Ako skener otisaka prstiju nije prikazan, a skener je integrisan u računar, idite na veb sajt proizvođača računara. U odeljku za tehničku podršku za model računara potražite Windows 10 upravljački program za skener koji možete da instalirate.

6. Ako je skener odvojen od računara (povezan putem USB),idite na veb sajt proizvođača skenera da biste pronašli i instalirali softver upravljačkog programa Windows 10 uređaja za model skenera koji imate.
