---
title: Pronalaženje IP adrese u evidenciji nadzora
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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902274"
---
# <a name="find-the-ip-address-in-audit-log"></a>Pronalaženje IP adrese u evidenciji nadzora

IP adresa koja odgovara aktivnosti koju je izvršio korisnik ili administrator prikazana je u evidencijama nadzora. Informacije o klijentu su takođe evidentirane. Evo kako da identifikujete IP adresu:

1. Uradite nešto od sledećeg:
   - Na Microsoft 365 centar za usaglašenost <https://compliance.microsoft.com> , idite na Nadzor  \> **rešenja**. Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 zaštitnik , <https://security.microsoft.com> idite na Nadzor . Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Ako vidite obaveštenje da treba da uključite nadzor, uključite ga odmah. Ako ova funkcija nije omogućena, rezultati pretrage neće moći da povlače podatke iz prethodnih datuma.

2. Na stranici **Nadzor** potvrdite da je **izabrana** kartica Pretraga, a zatim konfigurišite sledeće postavke:
   - **Opseg datuma i vremena:** Izaberite opseg datum/vreme u pocima **Početak** **i** Kraj.
   - **Aktivnosti:** Ako ste zainteresovani za određenu aktivnost, izaberite je sa liste; U suprotnom, **podrazumevana vrednost Prikaži rezultate za** sve aktivnosti vratiće se sve aktivnosti. Imajte na raspolaganju određene aktivnosti za izbor; međutim, te stavke nadzora će biti **vraćene ako se izabere stavka Prikaži rezultate** za sve aktivnosti.
   - **Korisnici:** Prihvatite praznu podrazumevanu vrednost da biste vratili rezultate za sve korisnike ili unesite jednog korisnika ili više njih.

3. Kada završite, kliknite na dugme **Pretraži**. Aktivnosti se pojavljuju na novoj stranici **Pretraga nadzora.**

4. U rezultatima izaberite stavku **Filtriraj rezultate** i **otkucajte Set-Mailbox** u polju filtera aktivnosti.

5. Izaberite zapis nadzora u rezultatima da biste otvorili **iskačeći** prozor Detalji.

Više informacija potražite u video zapisu [Pretraga evidencije nadzora da biste istražili uobičajene probleme sa podrškom.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
