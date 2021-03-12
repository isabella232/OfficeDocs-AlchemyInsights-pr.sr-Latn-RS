---
title: Popravka pravila transporta
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750576"
---
# <a name="fix-transport-rules"></a>Popravka pravila transporta

Pravilo za Prilagođeno slanje pošte utiče na ovu poruku. Da biste redigovali tačno pravilo, uradite sledeće:

1. U rezultatima prosleđivanja, u okviru **dodatne informacije** zabeležite **GUID** ili **ime smernica**.
2. Pokrenite Exchange Management Shell. Više informacija potražite u članku [Otvaranje programskog dodatka Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Pokrene ovu komandu (pomoću GUID-a sa vaše prosleđivanja):  **"Uzmi-TransportRule-identitet" GUID "| FL * opis***
4. Pregledajte opis da biste videli podešene uslove koji utiču na poruku.

Da biste saznali više, pogledajte članak [transport](https://go.microsoft.com/fwlink/?linkid=2101523).
