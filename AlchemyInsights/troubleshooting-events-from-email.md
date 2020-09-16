---
title: Rešavanje problema sa e-poštom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658748"
---
# <a name="troubleshooting-events-from-email"></a>Rešavanje problema sa e-poštom

1. Potvrdite da je funkcija omogućena za poštansko sanduče: **da biste dobili-Eventsfromemail Configuration <mailbox> – identitet**

2. Zatim pogledajte "događaji iz e-pošte" evidentira **Export-Mailboxdijagnostičke zapise <mailbox> – vremenski profil komponente**

3. U evidenciji "događaji iz e-pošte" Pronađite aplikaciju Internegeid koja se podudara sa stavkom u poštanskom sandučetu.  

4. Vrednost "pouzdanost" određuje da li se stavka dodaje ili ne. Događaji će biti dodati samo ako je vrednost "Pouzdani" = "pouzdan".

Vrednost "pouzdanost" određuje SPF, Dkim ili Dmark svojstva koja se nalaze u zaglavlju poruke.

Da biste prikazali ova svojstva:

**Outlook za stone računare**

- Otvaranje stavke
- Svojstva >-> Internet zaglavlja

Jer

**MFCMapi**

- Idite do stavke u prijemnom poštanskom sandučetu
- Potražite PR_TRANSPORT_MESSAGE_HEADERS_W

Ova svojstva su rešena i snimljena tokom transporta i proizvodnog postupka. Da biste mogli da rešite problem, možda ćete morati da izvršite pretraživanje sa podrškom za transport o neuspesima u programu SPF, DKIM i. ili DMARK.