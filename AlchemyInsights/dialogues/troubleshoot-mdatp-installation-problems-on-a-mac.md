---
title: Rešavanje problema sa programom MDATP instalacija na Mac računaru
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696094"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Rešavanje problema sa programom MDATP instalacija na Mac računaru

Ako Ručno instaliranje ne uspe, **stranica čarobnjaka** za instalaciju prikazuje sledeću grešku:

"Došlo je do greške tokom instalacije. Instalacioni program je naišao na grešku koja je izazvala otkazivanje instalacije. Obratite se proizvođaču softvera za pomoć. "

Za primena MDM-a, na stranici se prikazuje i Opšta greška.

Iako ne prikazujemo tačne greške za krajnji korisnik, zadržavamo datoteku evidencije sa napretkom instalacije, u **/Biblioteary/Logs/Microsoft/mdatp/Install.log**. Svaka sesija instalacije se dodaje na ovu datoteku evidencije. Da biste mogli da izvezete samo poslednju sesiju instalacije, koristite ih `sed` .

Da biste saznali više, pogledajte članak [Rešavanje problema sa instalacijom za ATP za Mac Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2144615).
