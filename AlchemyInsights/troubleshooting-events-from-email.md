---
title: Rešavanje problema sa događajima iz e-pošte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105366"
---
# <a name="troubleshooting-events-from-email"></a>Rešavanje problema sa događajima iz e-pošte

1. Provera da li je funkcija omogućena za poštansko sanduče: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Zatim pogledajte evidenciju "Događaji iz **e-pošte" evidencije Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. U evidencijama "Događaji iz e-pošte" pronađite InternetMessageId koji se podudara sa stavkom u poštanskom sandučetu.  

4. TrustScore određuje da li je stavka dodata ili ne. Događaji će se dodati samo ako je TrustScore = "Trusted".

Svojstva TrustScore određuju SPF, Dkim ili Dmarc svojstva koja se nalazi u zaglavlju poruke.

Da biste prikazali ova svojstva:

**Radna Outlook**

- Otvaranje stavke
- Svojstva datoteke > -> internet zaglavljima

ili

**MFCMapi**

- Prelaženje do stavke u prijemnom poštanskom sandučetu
- Potraži PR_TRANSPORT_MESSAGE_HEADERS_W

Ova svojstva se određuju i zapisuju tokom prenosa i usućivanja. Da biste dodatno rešavali probleme, možda ćete morati da pratite podršku za prenos o greškama u spF, DKIM i.ili DMARC-u.