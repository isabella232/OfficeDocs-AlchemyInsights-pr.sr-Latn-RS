---
title: Popravljanje smernica povezivanja
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988145"
---
# <a name="fix-connection-policy"></a>Popravljanje smernica povezivanja

E-poruka je označena kao bezbedna i isporučena u prijemno sanduče korisnika zato što je IP adresa koja se šalje označena kao bezbedna u smernicama filtera veze. Da biste pregledali smernice, uradite sledeće:

1. Idite u Office 365 centar za [&](https://go.microsoft.com/fwlink/p/?linkid=2077143)usaglašenost, a zatim idite u centar za borbu protiv bezb.  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Na kartici **Prilagođeno** izaberite smernicu **filtera veze**, a zatim izaberite stavku **Uredi smernicu**.
3. Pregledajte **listu dozvoljenih IP** adresa. Pogledajte da **Sef je** lista omogućena.

    > [!NOTE]
    > Microsoft se pretplati na izvore pouzdanih pošiljalaca nezavisnih dobavljača. Ako **Sef lista,** ti pouzdani pošiljalaci neće biti greškom označeni kao spam. Preporučujemo da izaberete ovu opciju zato što će smanjiti broj potvrđenih potvrđenih informacija (dobra pošta koja se klasifikova kao slanje pošte) koju primate.
