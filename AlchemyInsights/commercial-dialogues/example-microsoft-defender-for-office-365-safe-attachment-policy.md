---
title: Primer Microsoft Defender za Office 365 smernice za bezbedne priloge
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749198"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Primer Microsoft Defender za Office 365 smernice za bezbedne priloge

Ove postavke omogućavaju smernice pod imenom *bez kašnjenja* koje odmah šalju poruke, a zatim ponovo prilaže priloge posle skeniranja:

- **Ime**: nema kašnjenja
- **Opis**: dostavlja poruke odmah i ponovo prilaže priloge posle skeniranja.
- **Odgovor**: izaberite opciju **Dinamičko** rešenje. Više informacija potražite u članku [Dinamičko isporučivanje u smernicama bezbednog priloga](https://go.microsoft.com/fwlink/?linkid=2092328).
- Odeljak " **Preusmeravanje priloga** ": izaberite opciju **Omogućavanje preusmeravanja**, a zatim unesite e-adresu Microsoft 365 globalnog administratora, administratora bezbednosti ili analitičara koji će istražiti zlonamerne priloge.
- **Primeni na** odeljak: izaberite **domen primaoca**, a zatim izaberite domen. Izaberite stavku **Dodaj**, a zatim kliknite na **dugme u redu**. Kada završite, izaberite stavku **Sačuvaj**.

Da biste saznali više, pogledajte odeljak [bezbedni prilozi u programu Microsoft zaštitnik za Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
