---
title: 0x8004de40 greške prilikom pokretanja oneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813666"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 greške prilikom pokretanja oneDrive

Ako dobijete poruku o **grešci 0x8004de40** se pri prijavci u OneDrive, ponovootkucajte računar dok ste povezani sa poslovnim ili školskim domenom. Ako dobijete ovu grešku nakon ponošanja, pokušajte ovo dok ste povezani sa poslovnim ili školskim domenom:

1. Kliknite na dugme Start i  u polju za pretragu otkucajte **cmd** ili komandnu liniju, kliknite desnim tasterom miša na aplikaciju komandne linije i izaberite stavku Pokreni **kao administrator**. Ako budete upitani za administratorsku lozinku ili za potvrdu, otkucajte lozinku ili kliknite na dugme **Dozvoli.**  

2. U prozoru komandne linije otkucajte **dsregcmd /leave**  i sačekajte da se komanda dovrši. Zatim **otkucajte dsregcmd /join** i sačekajte da se komanda dovrši.
3. Ponovo poništite računar.
