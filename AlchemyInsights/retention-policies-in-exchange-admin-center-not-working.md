---
title: Smernice za zadržavanje u Exchange centru aktivnosti ne rade
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952242"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Smernice za zadržavanje u Exchange centru administrovanja

Ako želite da pokrenemo automatske provere postavki koje su pomenute ispod, kliknite na dugme "nazad< – na vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema sa smernicama za zadržavanje.

Ako imate problema sa smernicama za zadržavanje u Exchange centru adminimenata koje se ne primenjuju na poštanske sandučiće ili stavke koje se ne premeštaju u arhivski poštansko sanduče, proverite sledeće:

**Osnovni uzroci:**

- **Pomoćnik za kontrolisane** fascikle nije obradio poštansko sanduče korisnika. Pomoćnik za kontrolisane fascikle pokušava da obradi svako poštansko sanduče u organizaciji zasnovanoj na oblaku na svakih sedam dana.

  **Rešenje:** Pokrenite pomoćnik za kontrolisane fascikle.

- **ZadržavanjeHold je** **omogućeno u** poštanskom sandučetu. Ako je poštansko sanduče postavljeno na zadržavanje, smernice za zadržavanje poštanskog sandučeta neće biti obrađene tokom tog vremena.

  **Rešenje:** Proverite status postavke zadržavanja i ažurirajte po potrebi. Detalje možete da vidite u [temi Zadržavanje poštanskog sandučeta.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)
 
**Napomogućeno:** Ako je poštansko sanduče manje od 10 MB, pomoćnik za kontrolisane fascikle neće automatski obraditi poštansko sanduče.
 
Više informacija o smernicama za zadržavanje u Exchange centru admin center potražite u članku:

- [Oznake za zadržavanje i smernice za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [Primena smernica za zadržavanje na poštanske](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) sandučiće ili [Dodavanje ili uklanjanje oznaka zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [Kako da identifikujete tip zadrške postavljene u poštansko sanduče](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
