---
title: Otkazivanje rezervata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807991"
---
# <a name="cancelling-reservation"></a>Otkazivanje rezervata

- **Samouusluga:** Rezervisanu instancu možete da otkažete ili da je razmenjujete pomoću [Azure portala](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izaberite rezervaciju i kliknite na povraćaj ili Exchange. Imajte u vidu da morate da imate pristup vlasniku u nalogu za rezervaciju da biste razmenili ili vratili povraćaj. Pristup samo rezervatu vam neće dozvoliti da nastavite sa povraćajem i Exchange serverom. Zamolite vlasnika naloga za rezervacije da vam pruži vlasniku pristup nalogu rezervacije
- **Smernice za Exchange:** Možete da zamenite rezervaciju za drugu rezervaciju iste vrste – nema **kazni** za razmenu rezervacija. Ukupna posvećenost novoj rezervaciji treba da bude veća od sume razmenjene uplate rezervacija i budućih mesečnih uplata (ako je primenljivo)
- **Smernice za povraćaj povraćaja:** Zbir refundacije i otkazanih budućih uplata ne mogu da premašuju $50.000 USD u 12-mjesečnom iskačućem prozoru. **Trenutno ne naplaćujemo nikakvu kaznu** za povraćaj novca, ali možemo da joj naplatimo za buduće povraćaj fondova  
    **Izuzeci:** Samouslužni Exchange i otkazivanje mogućnosti nisu dostupne za klijente AMERIČKOG vladinog sporazuma
- Podrška za **API/PS/CLI** nije dostupna za ukidanje [samouslužnog rada i povraćaj finansijskih usluga za Azure rezervacije](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samouslužni Exchange i otkazivanje mogućnosti nisu dostupne za klijente AMERIČKOG vladinog sporazuma. Podržani su i drugi tipovi e-pošte koji uključuju Pay-as-go i CSP

Saznajte više: [Kako se obrade povratna i Exchange transakcije](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Saznajte više: [smernice za razmenu i povraćaj povraćaja](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Druga pitanja: [posjetiti rezervisane dokumente instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Razmena postojeće rezervisane instance (samouslužno)**

Možete da zamenite rezervaciju za novu rezervaciju iste vrste. Rezervaciju možete da vratite i do $50.000 USD godišnje, ako vam više nije potrebna. Samouslužni Exchange i otkazivanje mogućnosti nisu dostupne za klijente AMERIČKOG vladinog sporazuma. Podržavaju se i drugi tipovi američkih vlada koji uključuju Pay-as-go i CSP. Da biste Exchange ili refundiranje postojeće rezervacije, morate imati pristup vlasniku.

Sledeći koraci će voditi proceduru za dovršavanje transakcije

1. Prijavite se na [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izaberite rezervacije koje želite da ponovo vratite i kliknite na dugme **Exchange**
2. Izaberite tip proizvoda koji želite da kupite i otkucajte količinu. Uverite se da je nova ukupna vrednost kupovine veća od ukupnog zbira [određuje odgovarajuću veličinu pre kupovine](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Redigovanje i dovršavanje transakcije

**Povraćaj sredstava za rezervisanu instancu**

Da biste vratili povraćaj rezervata, idite na **detalje** i izaberite stavku **povraćaj novca**

**Procijenjen povraćaj nivoa:**

**Primerci i primeri minimalnog zahteva za povraćaj i razmenu**  
Primer rezervata rezervacije:

- Kupujete jednogodišnji IT za $120 u 1 januaru
- 7 aprila želite da vratite povraćaj ili zamenite ovu rezervaciju
- Pošto je rezervacija uživo za 97 dana, imaćete (1-97/365) * $120 nazad. (tj. $88,1). Trenutno ne postoji kazna za povraćaj
- Ako je razmena, nova kupovina bi trebalo da bude veća od $88,1
- Trenutno ne postoji kazna za povraćaj novca

**Primer rezervacije plana naplate:**

- Kupujete jednogodišnji IT za $10 mesečno
- 7 aprila želite da vratite povraćaj ili zamenite ovu rezervaciju
- Od poslednjeg plaćanja koji se dogodio 7 dana, imaćete (1-7/31) * $10 nazad. (tj. $7,74)
- Buduća ukinuta uplata je $80. Trenutno ne postoji kazna za povraćaj
- Otkazivanje ovog otkazivanja će $87,74 od vas je $50.000 ograničenje za povraćaj
- Ako razmena, ukupna vrednost nove kupovine treba da bude veća od $87,74

**Preporučeni dokumenti**

- [Kako se obrade povratna i Exchange transakcije](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Smernice za razmenu i povraćaj povraćaja](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)