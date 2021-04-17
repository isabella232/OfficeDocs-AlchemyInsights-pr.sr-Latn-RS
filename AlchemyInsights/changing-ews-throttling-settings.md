---
title: Promena postavki EWS ograničavanja
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818050"
---
# <a name="changing-ews-throttling-settings"></a>Promena postavki EWS ograničavanja

Pokrenite automatizovani test koji će vam omogućiti da izmenite smernice EWS ograničavanja tokom migracije. Imajte na umu da čak i nakon ovog pokretanje EWS uvoz će i dalje biti ograničen na 150 MB na 5 minuta po poštanskom sandučetu. Da biste postigli veću brzinu preuzimanja migracije, migrirajte više korisnika istovremeno.

Imajte na umu da promene smernica EWS ograničavanja ne utiču na sledeće tipove migracije (pomoću Microsoft alatki): hibridna, potpuna/fazna (RPC/HTTP), IMAP, G Suite, javna fascikla ili usluga PST uvoza.