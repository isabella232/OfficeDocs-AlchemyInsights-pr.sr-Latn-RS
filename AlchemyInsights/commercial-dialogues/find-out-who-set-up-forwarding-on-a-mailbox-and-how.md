---
title: Saznajte ko je postavio prosleđivanje u poštanskom sandučetu i kako
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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895193"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Saznajte ko je postavio prosleđivanje u poštanskom sandučetu i kako

Ako je spoljno prosleđivanje podešeno u poštanskom sandučetu, aktivnost se nadgleda u sklopu cmdlet stavke **Set-Mailbox** cmdlet. Evo kako da pronađete aktivnost u evidenciji nadzora:

1. Uradite nešto od sledećeg:
   - Na Microsoft 365 centar za usaglašenost <https://compliance.microsoft.com> , idite na Nadzor  \> **rešenja**. Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 zaštitnik , <https://security.microsoft.com> idite na Nadzor . Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://security.microsoft.com/auditlogsearch> .

   > [!NOTE]
   > Ako vidite obaveštenje da treba da uključite nadzor, uključite ga odmah. Ako ova funkcija nije uključena, rezultati pretrage neće moći da povlače podatke iz prethodnih datuma.

2. Na stranici **Nadzor** potvrdite da je **izabrana** kartica Pretraga, a zatim konfigurišite sledeće postavke:
   - Izaberite opseg datuma/vremena u **pocima Početak** **i** Kraj.
   - Potvrdite **da polje Aktivnosti** sadrži **opciju Prikaži rezultate za sve aktivnosti.**

3. Kada završite, kliknite na dugme **Pretraži**. Aktivnosti se pojavljuju na novoj stranici **Pretraga nadzora.**

4. U rezultatima kliknite na kolonu **Aktivnost** da biste sortirajli rezultate i pogledajte **stavku Podesi stavke poštanskog** sandučeta.

5. Izaberite aktivnost u rezultatima da biste otvorili letak sa detaljima. Morate da pogledate detalje svakog zapisa nadzora da biste utvrdili da li je aktivnost povezana sa prosleđivanju e-pošte:
   - **ObjectId:** Pseudonim vrednosti poštanskog sandučeta koje je izmenjeno.
   - **Parametri:** _ForwardingSmtpAddress ukazuje_ na ciljnu e-adresu.
   - **UserId:** Korisnik koji je konfigurovao prosleđivanje e-pošte u poštanskom sandučetu u **polju ObjectId.**

Dodatne informacije potražite u [temi "Odlučivanje o tome ko je podesio prosleđivanje e-pošte za poštansko sanduče"](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
