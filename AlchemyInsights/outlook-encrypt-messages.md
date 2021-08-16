---
title: S/MIME u Outlook na vebu
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
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010738"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifrovanje e-poruka u Outlook

Microsoft 365 Šifrovanje poruka je ugrađeno u Microsoft Azure Rights Management (Azure RMS), koji je deo usluge Azure Information Protection. Ako vaša pretplata uključuje Azure Rights Management ili Azure Information **Protection,** ne morate da preduzmete nikakve radnje da biste ručno omogućili ili aktivirali Uslugu Rights Management.

Na osnovu povratnih informacija klijenata, više nećemo omogućavati Exchange pravila za protok pošte da automatski šifruju odlaznu e-poštu koja sadrži određeni tip osetljivih informacija u zakupca. Umesto toga, pružamo detaljna uputstva o tome kako to možete da uradite. Dodatne detalje o tome kako da kreirate pravilo za prenos za šifrovanje osetljivih informacija potražite u [ovom članku.](https://aka.ms/OmeEtr)

- Ako koristite Outlook na vebu (ranije **OWA**): prilikom sastavljanja e-poruke, jednostavno kliknite na dugme Zaštiti **u** programu OWA. Ovo će primeniti dozvolu "Ne prosleđivati". Izaberite **stavku Promena dozvole** i **odaberite stavku** Šifruj da biste samo šifrovali poruku.

- Ako koristite **Outlook**: Da biste poslali šifrovanu poruku iz programa Outlook 2013 ili 2016 ili Outlook 2016 za Mac, izaberite Opcije Dozvole , a zatim izaberite opciju zaštite koja vam je  >  potrebna.

- Da **biste automatski šifrovali** sve e-poruke poslate određenim primaocima ili spoljnim partnerima, morate da kreirate pravilo za prenos protoka pošte u Exchange centru za administance. Detaljna uputstva su navedena u ovom [članku podrške.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

