---
title: Smernice za zadržavanje Exchange centru za administaciju ne rade
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074946"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Smernice za zadržavanje u Exchange centru za administrovanje

Ako želite da pokrenemo automatske provere postavki koje su pomenute ispod, kliknite na dugme "nazad< – na vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema sa smernicama za zadržavanje.

Ako imate problema sa smernicama za zadržavanje u Exchange centru aktivnosti koji se ne primenjuju na poštanske sandučiće ili stavke koje se ne premeštaju u arhivski poštansko sanduče, proverite sledeće:

**Osnovni uzroci:**

- **Pomoćnik za kontrolisane** fascikle nije obradio poštansko sanduče korisnika. Pomoćnik za kontrolisane fascikle pokušava da obradi svako poštansko sanduče u organizaciji zasnovanoj na oblaku na svakih sedam dana.

  **Rešenje:** Pokrenite pomoćnik za kontrolisane fascikle.

- **ZadržavanjeHold je** **omogućeno u** poštanskom sandučetu. Ako je poštansko sanduče postavljeno na zadržavanje, smernice za zadržavanje poštanskog sandučeta neće biti obrađene tokom tog vremena.

  **Rešenje:** Proverite status postavke zadržavanja i ažurirajte po potrebi. Detalje možete da vidite u [temi Zadržavanje poštanskog sandučeta.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Napomogućeno:** Ako je poštansko sanduče manje od 10 MB, pomoćnik za kontrolisane fascikle neće automatski obraditi poštansko sanduče.
 
Dodatne informacije o smernicama za zadržavanje u Exchange centru za administaciju potražite u članku:

- [Oznake za zadržavanje i smernice za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Primena smernica za zadržavanje na poštanske](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) sandučiće ili [Dodavanje ili uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Kako da identifikujete tip zadrške postavljene u poštansko sanduče](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
