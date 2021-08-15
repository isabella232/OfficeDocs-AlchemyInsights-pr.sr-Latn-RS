---
title: Konfigurisanje usluge obezbeđivanja
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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033292"
---
# <a name="configuring-the-provision-service"></a>Konfigurisanje usluge obezbeđivanja

Da bi automatizovano obezbeđivanje korisnika radilo, Azure AD zahteva važeće akredicije koji mu omogućavaju da se poveže sa API-jem veb usluga radnog dana. Pored toga, proverite vezu tokom radnog dana sa aplikacijom AD User Provisioning takođe proverava da li može da se poveže sa Azure AD Povezivanje agentom za obezbeđivanje povezanom sa AD domenom.

Ako Azure portal vraća grešku posle čuvanja akreditiva, pratite preporučene korake u nastavku:

1. Potvrdite da ste konfigurisali korisnički nalog sistema integracije za radni dan kao što je objašnjeno u odeljku uputstva Konfigurisanje korisnika sistema integracije u [radnom danu.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. Potvrdite da je usluga Azure AD Povezivanje obezbeđivanja usluge obezbeđivanja pokrenuta na vašem Windows serveru koristeći Services Management Console. Status agenta možete da proverite i na Azure portalu tako što ćete kliknuti na dugme Prikaži agente.
3. Uverite se da unosite vrednost za polje "Radno korisničko ime" koristeći format username@workday ime-zakupaca. Ako nedostaje ime zakutca za radni dan, potvrda identiteta iz radnog dana ne uspeva.
4. Ako konfigurizujete integraciju sa zakupnikom radne dana primene, primetićete zakazane nevremene u zakupca radnog dana. Radni dan je isplanirao neometano vreme za zakučare za primenu tokom vikenda (obično od petka večeri do subote ujutro), a otkazivanja povezivanja tokom ovog prozora vremena rada je poznat problem koji se automatski rešava čim zakučari primene ponovo dospeju na mrežu.
5. U retkim slučajevima, možete da vidite ovu grešku i ako se lozinka korisnika sistema integracije promeni zbog osvežavanja zakupita ili ako je nalog zaključan ili istekao. Proverite status korisnika sistema integracije sa administratorom radnog dana.

Više detalja o konfigurisanju radnog dana za automatizovano dodeljanje, pogledajte Uputstvo: Konfigurisanje radnog dana za automatsko [dodeljanje korisnika.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
