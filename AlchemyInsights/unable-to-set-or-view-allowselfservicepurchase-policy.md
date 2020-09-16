---
title: Nije moguće postavljanje ili prikaz smernice za Allowselfnabavka.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735213"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Nije moguće postavljanje ili prikaz smernice za Allowselfnabavka.

Kada pokušate da postavljate ili prikazujete smernice za Allowselfusluge, dobijate sledeću poruku o grešci:

*Ruguerror: nije uspelo preuzimanje smernica za proizvode sa šifrom polise "Allowselfservicenabavka", ErrorMessage – osnovna veza je zatvorena: došlo je do neočekivane greške na slanju.*

To je možda zbog starije verzije sistema Security Layer (TLS). Da biste povezali MSCommerce uslugu, morate da koristite TLS 1,2 ili noviji.  

Isprobajte sledeće korake da biste omogućili/odredili TLS protokol u 1,2, Verifikujte i pokušajte ponovo.
 1. Na komandnoj liniji PowerShell (PS C: \) Unesite sledeću komandu da biste na verziju 1,2 odredili TLS protokol:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Potvrdite TLS protokol u upotrebi sa sledećim komandama:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Ponovo pokušajte da izvršite kreiranje ili ažuriranje komandi po potrebi.

