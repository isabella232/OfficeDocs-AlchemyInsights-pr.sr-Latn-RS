---
title: Korišćenje Vix Veb lokacije sa sistemom Office 365 kupljenim ili upravljanim domenima
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300734"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korišćenje Vix Veb lokacije sa sistemom Office 365 kupljenim ili upravljanim domenima

- [Ažurirajte DNS zapise da biste zadržali Veb lokaciju sa trenutnim dobavljačem hostinga](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix članak "povezivanje domena sa programom wix pomoću metoda pokazivača" preporučuje se korišćenje pokazivača (dodavanje DNS zapisa po gornjoj vezi) umesto promene servera imena kada koristite Office 365
- Ako i dalje odaberete da promenite servere imena u wix, moraćete da  [KREIRATE DNS zapise u programu wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ako je vaš domen kupljen od korporacije Microsoft, ne može se promeniti serveri imena. Ako morate da promenite servere imena, Microsoft kupljeni domen treba da bude  [prebačen na drugi dobavljač usluga posle 60 dana](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)