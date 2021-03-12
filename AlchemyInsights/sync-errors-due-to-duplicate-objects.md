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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708076"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Greške pri sinhronizaciji zbog dupliranih objekata

Možete primiti jednu od sledećih poruka o grešci kada se sinhronizacija direktorijuma završi u programu Microsoft 365:

- Nije moguće ažurirati ovaj objekat u Microsoft usluzi na mreži zato što sledeći atributi povezani sa ovim objektom imaju vrednosti koji su možda već povezani sa drugim objektom u lokalnom direktorijumu.

- Sinhronizovani objekat sa istom proxy adresom već postoji u usluzi Microsoft Online Services.

- Nije moguće ažurirati ovaj objekat zato što sledeći atributi povezani sa ovim objektom imaju vrednosti koji su možda već povezani sa drugim objektom u lokalnim direktorijima: UserPrincipalName.

Da biste identifikovali i rešili problem, preuzmite i uradite alatku za rešavanje problema sa [Idfix DirSync](https://github.com/Microsoft/idfix).

Više informacija potražite u članku [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
