---
title: Popravljanje pravila prenosa
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034768"
---
# <a name="fix-transport-rules"></a>Popravljanje pravila prenosa

Ova poruka je uticala na prilagođeno pravilo protoka pošte. Da biste pregledali tačno pravilo, uradite sledeće:

1. U rezultatima prosleđivanja, u **okviru Dodatne** informacije pogledajte **GUID** ili **Ime smernica.**
2. Pokrenite Exchange Management Shell. Dodatne informacije potražite u [Exchange Upravljanje programom .](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Pokrenite ovu komandu (koristeći GUID iz  **prosleđivanje): Get-TransportRule -identity "GUID" | fl * Description***
4. Pregledajte opis da biste videli konfigurisane uslove koji utiču na poruku.

Da biste saznali više, pogledajte [get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
