---
title: Popravka smernica zakupca (zamena radnje)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748990"
---
# <a name="fix-tenant-policy-action-override"></a>Popravka smernica zakupca (zamena radnje)

Smernice za borbu protiv bezvredne pošte u zakupcu su pogođene ovom porukom. Da biste pregledali smernice, uradite sledeće:

1. Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim idite na smernice **za upravljanje pretnjama** za  >    >  [borbu protiv bezvredne pošte](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Potvrdite izbor u polju za proveru da li **izvor smernica** ukazuje na sledeće:  **Add-Xzaglavlje/ModifySubject/preusmeri/Izbriši/bez radnje/Bcc poruka**

    Ako je tako, na kartici **Prilagođeno** potvrdite postavke smernica koje utiču na poruku. Moguće je da su **standardne postavke** koje su primene na sve korisnike Exchange online zaštitnog klijenta pogođene porukom.

Više informacija o konfigurisanju smernica za filtriranje bezvredne pošte potražite u članku [Konfigurisanje smernica za filtriranje bezvredne pošte](https://go.microsoft.com/fwlink/?linkid=2101431).
