---
title: Greška 0x8004de40 prilikom pokretanja usluge OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823116"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>Greška 0x8004de40 prilikom pokretanja usluge OneDrive

Ako primite grešku **0x8004de40** prilikom prijavljivanja u OneDrive, ponovo pokrenite računar dok ste povezani sa poslovnim ili školskim domenom. Ako dobijete ovu grešku posle ponovnog pokretanja, isprobajte ovo povezivanje sa poslovnim ili školskim domenom:

1. Kliknite na dugme Start i otkucajte **cmd** ili **Komandna linija**  u polju za pretragu, kliknite desnim tasterom miša na aplikaciju komandne linije i izaberite stavku  **Pokreni kao administrator** . Ako vam bude zatraženo da dobijete administratorsku lozinku ili za potvrdu, otkucajte lozinku ili kliknite na dugme **Omogući** .  

2. U prozoru komandne linije otkucajte **dsregcmd/ostavi**  i sačekajte da se komanda dovrši. Zatim otkucajte **dsregcmd/JOIN** i sačekajte da se komanda dovrši.
3. Ponovo pokrenite računar.
