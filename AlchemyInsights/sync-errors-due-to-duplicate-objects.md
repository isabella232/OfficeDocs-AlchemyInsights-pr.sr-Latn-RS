---
title: 902 (greške sinhronizacije zbog dupliranih objekata)
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
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737355"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Greške pri sinhronizaciji zbog dupliranih objekata

Možete primiti jednu od sledećih poruka o grešci kada se sinhronizacija direktorijuma završi u programu Microsoft 365:

- Nije moguće ažurirati ovaj objekat u Microsoft usluzi na mreži zato što sledeći atributi povezani sa ovim objektom imaju vrednosti koji su možda već povezani sa drugim objektom u lokalnom direktorijumu.

- Sinhronizovani objekat sa istom proxy adresom već postoji u usluzi Microsoft Online Services.

- Nije moguće ažurirati ovaj objekat zato što sledeći atributi povezani sa ovim objektom imaju vrednosti koji su možda već povezani sa drugim objektom u lokalnim direktorijima: UserPrincipalName.

Da biste identifikovali i rešili problem, preuzmite i uradite alatku za rešavanje problema sa [Idfix DirSync](https://www.microsoft.com/download/details.aspx?id=36832).

Više informacija potražite u članku [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
