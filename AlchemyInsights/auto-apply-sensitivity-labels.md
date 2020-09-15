---
title: Automatsko Primenjivanje nalepnica sa senzitivnošću
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1737"
- "9000181"
ms.openlocfilehash: 8f316ad92ff31e28c3b3ffd25f25bd03ee159380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715179"
---
# <a name="auto-apply-sensitivity-labels"></a>Automatsko Primenjivanje nalepnica sa senzitivnošću

Oznake poverljivosti mogu ručno da se primene na sadržaj od strane korisnika ili možete da ih konfigurišete tako da se automatski primene na sadržaj.

Automatski primena nalepnica sa senzitivnošću uklanja potrebu za obukom korisnika o tome kako da klasifikuje sadržaj i potreba da ih obavesti o konfiguricijama smernica.

Da biste automatski primenili oznake, potrebno je sledeće:

- Usluge Azure usluge P2 pretplata
- [Preuzimanje i instaliranje programskog klijenta za zaštitu Azure informacija](https://docs.microsoft.com/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

Radimo na izvornoj podršci koja u budućnosti ne zahteva dodelu Azure-a za zaštitu podataka.

Trenutno samo Windows podržava jedinstvenog označavanja klijenta.  Funkcija još uvek nije podržana na Mac, iOS i android.

Više informacija o oznakama za osetljivost i primenite ih automatski na sadržaj, pogledajte članak:

- [Pregled oznaka osećajnosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)
- [Automatsko Primenjivanje oznake osetljivosti na sadržaj](https://docs.microsoft.com/office365/securitycompliance/apply_sensitivity_label_automatically)