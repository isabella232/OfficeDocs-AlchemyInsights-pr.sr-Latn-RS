---
title: Korišćenje Wix veb lokacije sa kupljenim ili kontrolisanim domenima usluge Office 365
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
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825961"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korišćenje Wix veb lokacije sa kupljenim ili kontrolisanim domenima usluge Office 365

- [Ažuriranje DNS zapisa da bi se zadržao veb sajt sa trenutnim dobavljačem usluge hostinga](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix članak "Povezivanje domena sa wix metodom" preporučuje da koristite pokazivač (dodavanje DNS zapisa po gorenavedenim vezama) umesto da menjate servere imena prilikom korišćenja usluge Office 365
- Ako i dalje odaberete da promenite servere imena na Wix, morate da kreirate DNS zapise na veb  [lokaciji Wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ako je domen kupljen od korporacije Microsoft, nije moguće promeniti servere imena. Ako morate da promenite servere imena, domen koji je kupio Microsoft moraće da se prenese drugom  [dobavljaču hostinga posle 60 dana](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)