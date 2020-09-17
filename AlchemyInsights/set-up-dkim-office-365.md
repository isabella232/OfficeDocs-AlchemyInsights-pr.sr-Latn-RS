---
title: Podešavanje DKIM
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808721"
---
# <a name="setup-dkim"></a>Podešavanje DKIM

Kompletna uputstva za konfigurisanje DKIM za prilagođene [domene](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)u programu Microsoft 365 su ovde.

1. Za **svaki** prilagođeni domen treba da kreirate **dva** dkim CNAME zapisa u usluzi DNS hostinga domena (obično je to registar domena). Na primer, contoso.com i fourthcoffee.com zahtevaju četiri DKIM CNAME zapisa: dva za contoso.com i dva za fourthcoffee.com.

   DKIM CNAME zapisi za **svaki** prilagođeni domen koriste sledeće formate:

   - **Ime hosta**: `selector1._domainkey.<CustomDomain>`

     **Upućuje na adresu ili vrednost**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Ime hosta**: `selector2._domainkey.<CustomDomain>`

     **Upućuje na adresu ili vrednost**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> je tekst sa leve strane `.mail.protection.outlook.com` u prilagođenom MX zapisu za prilagođeni domen (na primer, `contoso-com` za domen contoso.com). \<InitialDomain\> je domen koji ste koristili kada ste se prijavili za Microsoft 365 (na primer, contoso.onmicrosoft.com).

2. Kada kreirate CNAME zapise za prilagođene domene, dovršite sledeća uputstva:

   Neko. [Prijavite se u Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomoću poslovnog ili školskog naloga.

   -. Izaberite ikonu za pokretanje aplikacija u gornjem levom uglu i odaberite stavku **administrator**.

   trojku. U donjem levom oknu za navigaciju, razvijte stavku **administrator** i odaberite stavku **Exchange**.

   -. Idite na **bezbednost**  >  **dkim**.

   elektron. Izaberite domen, a zatim odaberite stavku **Omogućavanje** za **potpisivanje poruka za ovaj domen pomoću dkim potpisa**. Ponovite ovaj stepenik za svaki prilagođeni domen.
