---
title: Korišćenje Web lokacije wix sa Office 365 kupljenim ili kontrolisanim domenima
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
ms.openlocfilehash: 64dfe6082bea1e468eae78bf1576fde398e4c28a
ms.sourcegitcommit: 3ca312535d950105ee829e037f0ff8f1ddbbae72
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/11/2020
ms.locfileid: "44708499"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Korišćenje Web lokacije wix sa Office 365 kupljenim ili kontrolisanim domenima

- [Ažurirajte DNS zapise da biste zadržali Web lokaciju sa trenutnim dobavljačem hostinga](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix članak "povezivanje domena sa Skickom pomoću pokazivačkog metoda" preporučuje se korišćenje pokazivača (dodavanje DNS zapisa po gorenavedenoj vezi) umesto menjanja servera imena kada koristite Office 365
- Ako i dalje odaberete da promenite servere imena u wix, moraćete da [KREIRATE DNS zapise u wix-u za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ako je vaš domen nabavljen od korporacije Microsoft, serveri imena se ne mogu menjati. Ako morate da menjate servere za imena, Microsoft kupljeni domen će morati da bude [prebačen na drugog dobavljača usluga posle 60 dana](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider)