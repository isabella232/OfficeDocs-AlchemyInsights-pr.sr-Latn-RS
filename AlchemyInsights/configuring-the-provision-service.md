---
title: Konfigurisanje usluge odredbe
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484042"
---
# <a name="configuring-the-provision-service"></a>Konfigurisanje usluge odredbe

Za automatizovano obezbeđivanje rada na poslu, Azure AD zahteva važeće akreditive koje mu omogućuju da se poveže sa API-jem veb uslugama posla. Dodatno, dugme Testiraj vezu na radnom mestu za dodelu oglasa korisnika takođe proverava valjanost ako je u mogućnosti da se poveže sa agentom Azure AD Connect za obezbeđivanje povezivanja sa agentom za AD.

Ako Azure portal vraća grešku prilikom čuvanja akreditiva, slijedite sledeće navedene korake:

1. Potvrdite da ste podesili korisnički nalog sistema za integraciju u operativnom sistemu za integraciju kao što je navedeno u odeljku uputstvo [Konfiguriši korisnika sistema za integraciju u radnom toku](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Potvrdite da je usluga Azure veze za obezbeđivanje OGLAŠAVANJA uključena i da je pokrenuta na lokalnom Windows serveru pomoću konzole Management Console. Status agenta možete da potvrdite i tako što ćete kliknuti na dugme prikaz lokalnog agensa.
3. Uverite se da unosite vrednost za polje "korisničko ime radnog dana" pomoću formata username@workday-zakupca. Ako nedostaje radni dan-zakupac, potvrda radnog dana ne uspeva.
4. Ako podešavate integraciju sa zakupcem radnog dana, zabeležite planirana vremena za smanjenje radnog dana. Radni dan je već zakazao vreme za svoje stanare za implementaciju tokom vikenda (obično od petka uveče do subote ujutru) i problema sa povezivanjem tokom ovog prozora za smanjivanje je poznat problem koji se automatski rešava čim se svi stanari primene vrate na mreži.
5. U retkim slučajevima možete da vidite i ovu grešku ako je lozinka sistema za integraciju korisnik promenjen zbog osvežavanja zakupca ili ako je nalog u zaključanom ili isteklom stanju. Proverite status korisnika sistema za integraciju sa vašim radnim danom administratorom.

Za više detalja o konfigurisanju radnog vremena za automatizovano obezbeđivanje pogledajte [članak uputstvo: konfigurisanje radnog dana za automatsko obezbeđivanje korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
