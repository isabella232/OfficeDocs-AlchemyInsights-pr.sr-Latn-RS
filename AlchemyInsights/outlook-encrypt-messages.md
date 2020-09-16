---
title: S/MIME u programu Outlook na vebu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772312"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifrovanje e-poruka u programu Outlook

Šifrovanje usluge Microsoft 365 je ugrađeno u Microsoft Azure Rights Management (Azure RMS), koja je deo zaštite od Azure informacija. Ako pretplata sadrži Azure Rights Management ili bezbednost informacija, **Ne morate da preduzimate nikakve radnje da biste ručno omogućili ili aktivirali** uslugu Rights Management.

Na osnovu povratnih informacija o klijentu, više nećemo koristiti pravila razmene Exchange pošte da biste automatski šifrovali izlaznu e-poštu koja sadrži određene osetljive informacije u zakupcu. Umesto toga mi pružamo detaljna uputstva o tome kako to možete da uradite sami. Dodatne detalje o tome kako da kreirate pravilo za transport za šifrovanje osetljivih informacija potražite u [ovom članku](https://aka.ms/OmeEtr).

- Ako koristite Outlook na vebu (ranije **OWA**): prilikom sastavljanja e-poruke, jednostavno kliknite na dugme **zaštiti** u programu OWA. To će primeniti "ne Prosledi" dozvolu. Izaberite stavku **Promeni dozvolu** i odaberite stavku **šifrovanje** da biste šifruli poruku.

- Ako koristite **Outlook klijent**: da biste poslali šifrovanu poruku iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, **Izaberite stavku**  >  **dozvole**za zaštitu, a zatim izaberite opciju zaštite koja vam je potrebna.

- Da biste **automatski šifrovali sve e-poruke** poslate određenim primaocima ili spoljnim partnerskim organizacijama, potrebno je da kreirate pravilo za transport protoka pošte u Exchange centru administracije. Detaljna uputstva se pružaju u [ovom članku podrške](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

