---
title: Korišćenje opcije za otključavanje prsta u operativnom sistemu Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795258"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Korišćenje opcije za otključavanje prsta u operativnom sistemu Windows 10

**Omogućavanje Windows Zdravo otisaka prstiju**

Da biste otključali Windows 10 pomoću otiska prsta, morate da podesite Windows Helo otisak prsta tako što ćete dodati (dopustite da Windows nauči da prepoznaje) bar jedan prst. 

1. **Izaberite stavke postavke > nalozima > opcijama za prijavljivanje** (ili kliknite [ovde](ms-settings:signinoptions?activationSource=GetHelp)). Dostupne opcije za prijavljivanje će biti navedene. Na primer:

    ![Opcije prijavljivanja.](media/sign-in-options.png)

2. Kliknite ili dodirnite stavku **Windows Hello otisak prsta**, a zatim kliknite na dugme **Podesi**. U prozoru Podešavanje Windows Helo podešavanje kliknite na dugme **Prvi koraci**. Senzor otisaka prstiju će se aktivirati i bićete upitani da postavite prst na senzor:

   ![Senzor otisaka prstiju.](media/fingerprint-sensor.png)

3. Izvršite uputstva koja će zatražiti da vam više puta skenira prst. Kada se ovo završi, imaćete opciju dodavanja drugih prstiju koje ćete možda želeti da koristite za prijavljivanje. Sledeći put kada se prijavite u Windows 10, imaćete opciju korišćenja otiska prsta da biste to uradili.

**Windows Hello otisak prsta nije dostupan kao opcija za prijavljivanje**

Ako Windows Hello otisak prsta nije prikazan kao opcija u **opcijama za prijavljivanje**, to znači da Windows nije upoznat sa čitačem otisaka prstiju/skenerom priloženim na računaru ili da sistemska smernica sprečava njenu upotrebu (ako na primer, vašem računaru upravlja radno mesto). Da biste rešili problem: 

1. Kliknite na dugme **Start** na traci zadataka i potražite **Upravljač uređajima**.

2. Kliknite ili dodirnite da biste otvorili **Upravljač uređajima**.

3. U upravljaču uređajima, razvijte biometrijske uređaje tako što ćete kliknuti na njegov simbol.

   ![Biometrijski uređaji.](media/biometric-devices.png)

4. Skener otisaka prstiju trebalo bi da bude naveden kao biometrijski uređaj, kao što je čitač Sinapetika WBDI:

   ![Biometrijski uređaji.](media/biometric-devices-expanded.png)

5. Ako skener za otiske prstiju nije prikazan i ako je skener integrisan u računar, idite na Veb lokaciju proizvođača računara. U odeljku tehnička podrška za PC model potražite Windows 10 upravljački program za skener koji možete instalirati.

6. Ako je skener odvojen od računara (priložen pomoću USB-a), idite na Veb lokaciju proizvođača skenera da biste pronašli i instalirali softver za Windows 10 upravljački program za uređaj koji imate.
