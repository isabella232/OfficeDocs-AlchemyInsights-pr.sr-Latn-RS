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
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020206"
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

