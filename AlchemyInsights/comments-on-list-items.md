---
title: Komentari u stavkama liste
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995502"
---
# <a name="comments-on-list-items"></a>Komentari u stavkama liste

Korisnici mogu da vide sve komentare o stavci liste i da filtriraju između prikaza koji pokazuju komentare ili aktivnost povezane sa stavkom.

Korisnici treba da imaju utišane sledeće informacije da bi mogli da dodaju i izbrišu komentare:

- Komentari prate postavke dozvola nasledne u programu SharePoint.
- Klasične liste koje još nisu izgrađene za prikaz u modernom korisničkom interfejsu, kao što su liste zadataka, neće imati ovu funkciju za komentare.
- Komentarisanje lista u programu Teams nije dostupno uz ovo izdanje.
- Pretraga ne indeksira komentare.

Administracioni programi mogu da onemoguće ovu funkciju na nivou organizacije tako što će promeniti parametar **CommentsOnListItemsDisabled** u cmdlet komandi **Set-SPOTenant** PowerShell.

Trenutno nije moguće onemogućiti komentare na nivou sajta ili liste. Nadamo se da ćemo imati te kontrole u kasnijem ažuriranju, verovatno u prvom kvartalu 2021.
