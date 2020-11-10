---
title: Komentari na listi stavki
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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982559"
---
# <a name="comments-on-list-items"></a>Komentari na listi stavki

Korisnici će uskoro moći da dodaju i brišu komentare na stavkama liste. Korisnici mogu da pregledaju sve komentare na stavci liste i da filtriraju između prikaza koji prikazuju komentare ili aktivnosti povezane sa stavkom.

**Tajming** :

**Ciljano izdanje** : postepeno se vrti sredinom oktobra i očekuje se da će biti završen do sredine novembra

**Standardno izdanje** : postepeno se vrti u sredinom novembra i očekuje se da će biti završen početkom decembra

**Rollout** Prijem: ciljano izdanje za celu organizaciju

Korisnici treba da zabeležite sledeće pre nego što dodaju i brišu komentare:

- Komentari slede postavke dozvola koje su svojstvene u sistemu SharePoint.
- Klasične liste koje još uvek nisu ugrađene da se pojave u modernim korisničkim interfejsima, kao što su liste zadataka, neće imati ovu funkciju komentarišanje.
- Komentarišanje listi u timovima nije dostupno ovim izdanjima.
- Pretraživanje komentara nije Indeksirano.

Administratori mogu da onemoguće ovu funkciju na nivou organizacije tako što ćete promeniti parametar " **pohvalkalistitemsonemogućavanje** " **Set-SPOTenant** u PowerShell cmdlet usluzi.

Trenutno nije moguće onemogućiti komentarisanje na lokaciji ili nivou liste. Nadamo se da ćemo imati te kontrole u kasnijoj ispravci, verovatno u prvom kvartalu 2021.
