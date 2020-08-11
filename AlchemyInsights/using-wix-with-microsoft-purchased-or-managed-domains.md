---
title: Korišćenje wix Veb lokacije sa Microsoft kupljenim ili upravljanim domenima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: f6845c56f05e9cef11362ce601a974b73a154c9a
ms.sourcegitcommit: 28a319e482e6a8644e87726e1b0e599819df52d0
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2020
ms.locfileid: "46629836"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a>Korišćenje wix Veb lokacije sa Microsoft kupljenim ili upravljanim domenima

Informacije o tome kako da koristite wix Veb lokaciju pomoću Microsoft kupljenog ili kontrolisanog domena potražite [u članku ažuriranje DNS zapisa radi zadržavanja Veb lokacije kod trenutnog dobavljača usluga hostinga](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider).

Detalje potražite u članku: 

- Vix članak, "povezivanje domena sa Viksom pomoću metoda pokazivača", preporučuje se Dodavanje DNS zapisa kao što je navedeno u članku iznad, a ne za menjanje servera imena kada koristite Microsoft 365.

- Ako odaberete da promenite servere imena u Vix, morate da kreirate DNS zapise u programu wix za Microsoft. Više informacija potražite u članku [Kreiranje DNS zapisa na lokaciji wix za Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix).

- Ako je vaš domen kupljen od korporacije Microsoft, ne možete da promenite servere imena. Ako morate da promenite servere imena, Microsoft kupljeni domen mora biti prebačen na drugi dobavljač usluga posle 60 dana. Više informacija potražite u članku [najčešća pitanja o domenima](https://docs.microsoft.com/microsoft-365/admin/setup/domains-faq#can-i-transfer-a-domain-i-purchased-from-microsoft-to-another-provider).