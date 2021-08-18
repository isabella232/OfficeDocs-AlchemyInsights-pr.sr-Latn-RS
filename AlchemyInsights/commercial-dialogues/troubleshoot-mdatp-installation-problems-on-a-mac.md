---
title: Rešavanje problema sa MDATP instalacijom na Mac računaru
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
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091074"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Rešavanje problema sa MDATP instalacijom na Mac računaru

Ako ručna instalacija ne uspe, **stranica Rezime** čarobnjaka za instalaciju prikazuje sledeću grešku:

"Došlo je do greške tokom instalacije. Instalacioni program je naišao na grešku koja je dovela do neuspešne instalacije. Obratite se proizvođaču softvera za pomoć".

Za MDM primene stranica prikazuje i generičke greške pri instalaciji.

Iako ne prikazujemo tačne greške krajnjih korisnika, čuvamo datoteku evidencije sa tokom instalacije, u **/Library/Logs/Microsoft/mdatp/install.log.** Svaka sesija instalacije dodaje ovoj datoteci evidencije. Da biste izneli samo poslednju sesiju instalacije, koristite `sed` .

Da biste saznali više, pogledajte članak [Rešavanje problema sa instalacijom za Microsoft zaštitnik ATP za Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
