---
title: 0x8004de40 greške prilikom pokretanja OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946593"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 greške prilikom pokretanja OneDrive

Ako dobijete poruku o **0x8004de40** grešku prilikom prijavljivanje u OneDrive, ponovo ga poništite dok ste povezani sa poslovnim ili školskim domenom. Ako dobijete ovu grešku nakon ponošanja, pokušajte ovo dok ste povezani sa poslovnim ili školskim domenom:

1. Kliknite na dugme Start i  u polju za pretragu otkucajte **cmd** ili komandnu liniju, kliknite desnim tasterom miša na aplikaciju komandne linije i izaberite stavku Pokreni **kao administrator**. Ako budete upitani za administratorsku lozinku ili za potvrdu, otkucajte lozinku ili kliknite na dugme **Dozvoli.**  

2. U prozoru komandne linije otkucajte **dsregcmd /leave**  i sačekajte da se komanda dovrši. Zatim **otkucajte dsregcmd /join** i sačekajte da se komanda dovrši.
3. Ponovo poništite računar.
