---
title: Rešavanje problema sa e-poštom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569405"
---
# <a name="troubleshooting-events-from-email"></a>Rešavanje problema sa e-poštom

1. Proverite da li je omogućena funkcija za poštansko sanduče: **get-Eventsfromemailiskonfiguracija <mailbox> -identitet**

2. Zatim pogledajte ' događaje iz e-maila ' evidencije **Export-MailboxDiagnosticLogs <mailbox> -Component time profil**

3. U "događajima iz evidencije e-pošte", pronađite Internetporuku koja se podudara sa stavkom u poštanskom sandučetu.  

4. Rezultat Pover, određuje da li je artikal dodat ili ne. Događaji će biti dodati samo ako je poverljiv rezultat = "pouzdan".

Rezultat povernje je određen svojstvima SPF, Dkim ili Dmark, koji se nalaze u zaglavlju poruke.

Da biste prikazali ova svojstva:

**Radnu površinu Outlook**

- Otvorite stavku
- Svojstva > datoteke-> Internet zaglavlja

Ili

**MFCMapi**

- Kretanje do stavke u prijemnom poštanskom sandučetu
- Potraži PR_TRANSPORT_MESSAGE_HEADERS_W

Ova svojstva se određuju i zapisuju tokom transporta i proizvodnog postupka. Za dalje rešavanje problema, možda ćete morati da pratite podršku za transport u vezi sa otkazima u SPF-u, DKIM i. ili DMARK.