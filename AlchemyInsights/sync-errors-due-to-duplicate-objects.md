---
title: 902 (greške pri sinhronizaciji zbog dupliranih objekata)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998808"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Sinhronizovanje grešaka zbog dupliranih objekata

Možete da dobijete jednu od sledećih poruka o grešci kada se sinhronizacija direktorijuma završi u Microsoft 365:

- Nije moguće ažurirati ovaj objekat u Microsoft Online Services jer sledeći atributi povezani sa ovim objektom imaju vrednosti koje su možda već povezane sa drugim objektom u lokalnom direktorijumu.

- Sinhronizovani objekat sa istom proxy adresom već postoji u Microsoft Online Services direktorijumu.

- Nije moguće ažurirati ovaj objekat jer sledeći atributi povezani sa ovim objektom imaju vrednosti koje su možda već povezane sa drugim objektom u uslugama lokalnog direktorijuma: UserPrincipalName.

Da biste identifikovali i rešili problem, preuzmite i pokrenite alatku za popravljanje [IdFix DirSync grešaka.](https://github.com/Microsoft/idfix)

Dodatne informacije potražite u [temi KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
