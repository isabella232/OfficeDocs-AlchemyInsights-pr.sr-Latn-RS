---
title: Korišćenje Wix veb lokacije sa Office 365 kupljenim ili kontrolisanim domenima
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
ms.openlocfilehash: d7df06d768eabb44bcaee4a7450d16ecdb3395da4cee4810503d3dae358736ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53980191"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korišćenje Wix veb lokacije sa Office 365 kupljenim ili kontrolisanim domenima

- [Ažuriranje DNS zapisa da bi se zadržao veb sajt sa trenutnim dobavljačem usluge hostinga](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix članak "Povezivanje domena sa Wix mrežom pomoću metoda upućivanja" preporučuje da koristite pokazivač (dodavanje DNS zapisa po gorenavedenim vezama) umesto da menjate servere imena kada koristite Office 365
- Ako i dalje odaberete da promenite servere imena na Wix, morate da kreirate DNS zapise na veb  [lokaciji Wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ako je domen kupljen od korporacije Microsoft, nije moguće promeniti servere imena. Ako morate da promenite servere imena, domen koji je kupio Microsoft moraće da se prenese drugom  [dobavljaču hostinga posle 60 dana](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)