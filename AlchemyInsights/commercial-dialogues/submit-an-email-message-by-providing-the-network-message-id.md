---
title: Prosleđivanje e-poruke obezbeđivanje ID-a mrežne poruke
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929931"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Prosleđivanje e-poruke obezbeđivanje ID-a mrežne poruke

1. Na **iskusnu iskusnuće "Nova** poruka" izaberite stavku **ID** **e-pošte i mrežne poruke**.
2. Pratite ove korake da biste pronašli ID poruke za e-poruku u Outlook:
    1. Kliknite dvaput na e-poruku da biste je otvorili.
    1. Izaberite **stavku**  >  **Svojstva datoteke**.
    1. Otvorite Beležnica ili prazan Word dokument, a zatim kopirajte i nalepite sadržaj koji se nalazi u okviru **internet** zaglavlja u otvorenom dokumentu radi bolje vidljivosti.
    1. Pronađite **polje X-MS-Exchange-Organization-Network-Message-Id.** Vrednost posle **: je** ID potreban za prosleđivanje.
3. U **okviru Primaoci,** ako je e-pošta koja je došla u fasciklu neželjene pošte za sve primaoce ove e-poruke, odaberite **stavku Izaberi sve**. Ako nije, izaberite samo korisnika koji je prijavio problem.
4. U okviru Razlog za prosleđivanje **,** ako izaberete stavku Trebalo bi da je blokirano **,** navedite da li je poruka trebalo da se blokira kao Bez-pošta **,** **Phishing** ili **Malver**, a zatim izaberite Prosledi **.**

Da biste saznali više, pogledajte članak Kako da prosledite sumnjivu [bezbraznu pošiljku, phish, UL](https://go.microsoft.com/fwlink/?linkid=2101479)datoteke i datoteke korporaciji Microsoft u skeniranje.
