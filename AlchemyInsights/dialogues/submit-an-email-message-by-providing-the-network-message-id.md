---
title: Prosleđivanje e-poruke tako što će obezbediti ID mrežne poruke
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695383"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Prosleđivanje e-poruke tako što će obezbediti ID mrežne poruke

1. U **novom programu prosleđivanja** , izaberite stavku **e-pošta** i **ID poruke na mreži**.
2. Slijedite ove korake da biste pronašli ID poruke za e-poruku u programu Outlook:
    1. Kliknite dvaput na e-poruku da biste je otvorili.
    1. Izaberite stavku  >  **Svojstva** datoteke.
    1. Otvorite Notepad ili prazan Word dokument, a zatim kopiju i nalepite sadržaj koji se nalazi u okviru " **Internet zaglavlja** " u otvorenom dokumentu radi bolje vidljivosti.
    1. Pronađite polje **X-MS-Exchange-organizacija-ID-poruka** . Vrednost posle **:** predstavlja ID koji vam je potreban za prosleđivanje.
3. Ako je e-pošta sletela u fasciklu "Neželjena pošta" za sve primaoce ove e- **poruke, odaberite** **stavku "Izaberi sve**". Ako nije, izaberite samo korisnika koji je prijavio problem.
4. U okviru **razlog za prosleđivanje**, ako izaberete **treba da bude blokirano**, navedite da li je poruka trebalo da bude blokirana kao **bezvredna**, **phishing** ili **malver**, a zatim izaberite stavku **Prosledi**.

Da biste saznali više, pogledajte [Kako da prosledite osumnjičene bezvredne pošte, frish, URL adrese i datoteke korporaciji Microsoft za skeniranje](https://go.microsoft.com/fwlink/?linkid=2101479).
