---
title: Rešavanje smernica veze
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695886"
---
# <a name="fix-connection-policy"></a>Rešavanje smernica veze

E-poruka je označena kao bezbedna i isporučena u korisnički prijemno poštansko sanduče jer je IP adresa slanja označena kao bezbedna u smernicama za filtriranje veze. Da biste pregledali smernice, uradite sledeće:

1. Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim idite na smernice **za upravljanje pretnjama** za  >    >  [borbu protiv bezvredne pošte](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na kartici **Prilagođeno** izaberite **smernice za filtriranje veze**, a zatim izaberite stavku **Uredi smernice**.
3. Pregledajte listu **dozvole za IP** . Pogledajte članak da li je **Sigurnosna lista** omogućena.

    > [!NOTE]
    > Microsoft se pretplate na nezavisne pošiljaoce pouzdanih pošiljalaca. Ako je **bezbedna lista** omogućena, ovi pouzdani pošiljaoci nisu pogrešno označeni kao spam. Preporuиujem vam da izaberete ovu opciju jer će se smanjiti broj pogrešnih informacija (dobra pošta koja je klasifikovana kao bezvredna pošta) koju primate.
