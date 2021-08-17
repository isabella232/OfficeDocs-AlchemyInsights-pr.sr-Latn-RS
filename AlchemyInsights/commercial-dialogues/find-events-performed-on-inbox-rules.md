---
title: Pronalaženje događaja izvršenih na pravilima prijemnog poštanskog sandučeta
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882649"
---
# <a name="find-events-performed-on-inbox-rules"></a>Pronalaženje događaja izvršenih na pravilima prijemnog poštanskog sandučeta

Kada se kreiraju, menjaju ili brišu pravila prijemnog poštanskog sandučeta, događaji se snimaju u evidenciji nadzora. Evo kako da ih pregledate:

1. Uradite nešto od sledećeg:
   - Na Microsoft 365 centar za usaglašenost <https://compliance.microsoft.com> , idite na Nadzor  \> **rešenja**. Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 zaštitnik , <https://security.microsoft.com> idite na Nadzor . Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Ako vidite obaveštenje da treba da uključite nadzor, uključite ga odmah. Ako ova funkcija nije uključena, rezultati pretrage neće moći da povlače podatke iz prethodnih datuma.

2. Na **kartici Pretraga** na **stranici** Nadzor konfigurišite sledeće postavke:
   - **Opseg datuma i vremena:** Izaberite opseg datum/vreme u pocima **Početak** **i** Kraj.
   - **Aktivnosti: Odaberite** **stavku Novo prijemno poštansko sanduče Napravi pravilo prijemnog poštanskog sandučeta od Outlook Web App**

3. Kada završite, kliknite na dugme **Pretraži**. Aktivnosti se pojavljuju na novoj stranici **Pretraga nadzora.**

4. Izaberite aktivnost u rezultatima da biste otvorili letak sa detaljima. U **odeljku Parametri** možete da vidite ime pravila, skup uslova i radnje koje će pravilo preduzeti.

Da biste saznali više, pogledajte pretragu [evidencije nadzora da biste istražili uobičajene probleme sa podrškom.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
