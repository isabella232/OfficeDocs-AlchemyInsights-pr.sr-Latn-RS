---
title: Nije moguće podesiti ili prikazati smernice AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826105"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nije moguće podesiti ili prikazati smernice AllowSelfServicePurchase

Kada pokušate da postavite ili prikažete smernicu AllowSelfServicePurchase, dobijate sledeću poruku o grešci:

*HandleError: Nije uspelo preuzimanje smernica proizvoda sa SmernicomId "AllowSelfServicePurchase", ErrorMessage – Osnova veza je zatvorena: Došlo je do neočekivane greške prilikom slanja.*

To može da bude zbog starije verzije transport Layer Security (TLS). Da biste povezali uslugu MSCommerce, morate da koristite TLS 1.2 ili veću.  

Isprobajte sledeće korake da biste omogućili/postavili TLS protokol na 1.2, verifikujte i pokušajte ponovo.
 1. Na PowerShell komandnoj liniji (PS C: unesite sledeću komandu da biste postavili TLS protokol na \) verziju 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Potvrdite TLS protokole koji se koriste uz sledeću komandu:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Ponovo, po potrebi, ponovotrite komande Nabavi ili Ažuriraj.

