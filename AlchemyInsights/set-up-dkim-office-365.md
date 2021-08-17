---
title: Podešavanje DKIM-a
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108570"
---
# <a name="setup-dkim"></a>Podešavanje DKIM-a

Kompletna uputstva za konfigurisanje DKIM-a za prilagođene domene u Microsoft 365 su [ovde.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Za **svaki** prilagođeni domen morate da kreirate dva **DKIM** CNAME zapisa u usluzi DNS hostinga za domen (to je obično registar domena). Na primer, contoso.com i fourthcoffee.com zahtevaju četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.

   DKIM CNAME zapisi za **svaki prilagođeni** domen koriste sledeće formate:

   - **Ime hosta:**`selector1._domainkey.<CustomDomain>`

     **Upunjuje na adresu ili vrednost:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   - **Ime hosta:**`selector2._domainkey.<CustomDomain>`

     **Upunjuje na adresu ili vrednost:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   \<DomainGUID\> je tekst sa leve strane u prilagođenom MX zapisu za prilagođeni domen (na primer, za domen `.mail.protection.outlook.com` `contoso-com` contoso.com). \<InitialDomain\>je domen koji ste koristili kada ste se upisali za Microsoft 365 (na primer, contoso.onmicrosoft.com).

2. Kada kreirate CNAME zapise za prilagođene domene, dovršite sledeća uputstva:

   a. [prijavite se u Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) sa poslovnim ili školskim nalogom.

   b. Izaberite ikonu za pokretanje aplikacija u gornjem levom vremenu i **odaberite stavku Administ.**

   c. U navigaciji u donjem levom vremenu **razvijte stavku "Admin"** i **odaberite stavku Exchange.**

   d. Idite na **Zaštita**  >  **DKIM .**

   e. Izaberite domen, a zatim **odaberite stavku** Omogući **za potpisivanje poruka za ovaj domen sa DKIM potpisima**. Ponovite ovaj korak za svaki prilagođeni domen.
