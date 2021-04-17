---
title: Otkazivanje rezervacije
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819706"
---
# <a name="cancelling-reservation"></a>Otkazivanje rezervacije

- **Samouslužno:** Možete sami da otkažete ili zamenite rezervisanu instancu koristeći [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izaberite rezervaciju i kliknite na refundaciju ili razmenu. Imajte napominje da morate imati vlasnički u porudžbini rezervacije da biste zamenili ili refundirali. Pristup samo rezervaciji neće vam dozvoliti da nastavite sa refundacijom ili razmenom. Zamolite vlasnika naloga za rezervaciju da vam omogući vlasniku pristup nalogu za rezervaciju
- **Smernice razmene:** Možete zameniti rezervaciju za drugu rezervaciju istog tipa – **nema** kazne za zamenu rezervacije. Ukupna obaveza sa novom rezervacijom treba da bude veća od zbira iznosa refundacije zamenjene rezervacije i budućih mesečnih uplata (ako je primenljivo)
- **Smernice refundacije:** Zbir refundacije i otkazanih budućih uplata ne može premašiti 50 000 USD u 12-mesečnom sukcesivnom prozoru. Trenutno **ne naplaćujemo nikakve kazne za refundaciju**, ali bismo ih mogli naplatiti za buduće refundacije  
    **Izuzeci:** Mogućnost samoposlužne razmene i otkazivanja nije dostupna za klijente američkog vladinog ugovora
- **API / PS / CLI** podrška nije dostupna za otkazivanje i refundaciju [Samouslužne razmene i refundacije za Azure Rezervacije](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Mogućnost samouslužne razmene i otkazivanja nije dostupna za klijente američkog vladinog ugovora za preduzeća. Imajte na umu da morate imati vlasnički pristup na Nalogu za rezervaciju da biste ga zamenili ili vratili novac.

Saznajte više: [Kako se obrađuju transakcije povratka i razmene](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
Saznajte više: [Smernice za Razmenu i refundaciju](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Druga pitanja: [Posetite rezervisana dokumenta za instancu](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Razmeni postojeću rezervisanu instancu (Samouslužno)**

Rezervaciju možete zameniti za drugu rezervaciju istog tipa. Takođe možete refundirati rezervaciju, do 50.000 USD godišnje, ako vam više nije potrebna. Mogućnost samouslužne razmene i otkazivanja nije dostupna za klijente američkog vladinog ugovora za preduzeća. Podržani su i drugi tipovi pretplata američke vlade, uključujući plaćanje po utrošku i CSP. Morate imati vlasnički pristup na Nalogu za rezervaciju da biste zamenili ili refundirali postojeću rezervaciju.

Sledeći koraci će vas voditi kroz postupak dovršavanja transakcije

1. Prijavite se na svoj [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izaberite rezervacije koje želite da refundirate i kliknite na dugme **Exchange**
2. Izaberite VM proizvod koji želite da kupite i unesite količinu. Uverite se da je ukupan iznos nove kupovine veći od ukupnog unosa [Utvrdite željenu veličinu pre kupovine](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Pregledajte i dovršite transakciju

**Refundacija za rezervisanu instancu**

Da biste refundirali rezervaciju, idite na **Detalje rezervacije** i kliknite **Refundiraj**

**Proporcijalna refundacija:**

**Primeri proporcije i minimalnih zahteva za povraćaj sredstava i razmenu**  
Primer rezervacije unapred:

- Kupujete jednogodišnji RI za 120 USD 1. januara
- 7. aprila želite da refundirate ili zamenite ovu rezervaciju
- Pošto je rezervacija aktivna 97 dana, dobićete nazad (1-97/365) * 120 USD. (i.e. $88.1). Trenutno nema kazne za refundaciju
- Ako menjate, vaša nova kupovina bi trebala biti veća od 88,1 USD
- Trenutno nema kazne za povraćaj sredstava

**Primer rezervacije plana naplate:**

- Kupujete jednogodišnji RI za 10 dolara mesečno
- 7. aprila želite da refundirate ili zamenite ovu rezervaciju
- Pošto se poslednja uplata dogodila 7 dana, dobićete nazad (1-7/31) * 10 USD. (i.e. $7.74)
- Buduće otkazane uplate iznose 80 USD. Trenutno nema kazne za refundaciju
- Ovo otkazivanje oduzeće vam 87,74 USD sa ograničenja refundacije od 50 000 USD
- Ako menjate, ukupna vrednost vaše nova kupovine bi trebala biti veća od 87,74 USD

**Preporučeni dokumenti**

- [Kako se obrađuju transakcije povrata i razmene](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Smernice za Razmenu i refundaciju](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)