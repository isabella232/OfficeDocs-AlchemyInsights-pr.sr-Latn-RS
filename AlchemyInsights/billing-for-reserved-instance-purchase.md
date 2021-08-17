---
title: Naplata za kupovinu rezervisane instance
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104034"
---
# <a name="billing-for-reserved-instance-purchase"></a>Naplata za kupovinu rezervisane instance

Rezervisana kupovina instanci se naplaćuje načinom plaćanja koji je vezan za pretplatu koju ste izabrali u vreme kupovine. Tip pretplate mora da bude ugovor sa preduzećem (broj ponude: MS-AZR-0017P), Pay-As-You-Go (broj ponude: MS-AZR-0003P), Microsoft korisnički ugovor ili CSP.

- Za pretplatu na preduzeća, troškovi se oduzimaju iz salda monetarne obaveze upisa ili se naplaćuju kao prekomerno korišćenje
- Za pretplatu na Pay-As-Go, troškovi se naplaćuju na kreditnoj kartici ili načinu plaćanja po fakturi za pretplatu

**Otkazivanje rezervacije**

- **Samouslužno:** Možete sami da otkažete ili zamenite rezervisanu instancu koristeći [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izaberite rezervaciju i kliknite na refundaciju ili zamenu. Imajte na umu da morate imati vlasnički pristup u porudžbini rezervacije da biste obavili zamenu ili refundaciju. Pristup samo rezervaciji neće vam dozvoliti da nastavite sa refundacijom ili zamenom. Zamolite vlasnika porudžbine rezervacije da vam omogući vlasnički pristup porudžbini rezervacije
- **Smernice zamene:** Možete zameniti rezervaciju za drugu rezervaciju istog tipa – **nema** kazne za zamenu rezervacije. Ukupna obaveza sa novom rezervacijom treba da bude veća od zbira iznosa refundacije zamenjene rezervacije i budućih mesečnih uplata (ako je primenljivo)
- **Smernice refundacije:** Zbir refundacije i otkazanih budućih uplata ne može premašiti 50.000 USD u intervalu od 12 uzastopnih meseci. Trenutno **ne naplaćujemo nikakve kazne za refundaciju**, ali bismo ih mogli naplatiti za buduće refundacije

**Izuzeci:** Mogućnost samouslužne zamene i otkazivanja nije dostupna korisnicima Enterprise ugovora sa državnom upravom SAD

- **API / PS / CLI** podrška nije dostupna za otkazivanje i refundaciju [Samouslužne zamene i refundacije za Azure rezervacije](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Mogućnost samouslužne zamene i otkazivanja nije dostupna korisnicima Enterprise ugovora sa državnom upravom SAD. Podržani su drugi tipovi pretplata za državnu upravu SAD, uključujući plaćanje po utrošku i CSP

Saznajte više: Kako se obrađuju povratne i [exchange](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) transakcije Saznajte više: Exchange smernice za [povraćaj](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) novca Druga pitanja: Posetite rezervisane dokumente za [instancu](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Zameni postojeću rezervisanu instancu (samouslužno)**

Rezervaciju možete zameniti za drugu rezervaciju istog tipa. Takođe možete refundirati rezervaciju, do 50.000 USD godišnje, ako vam više nije potrebna. Mogućnost samouslužne zamene i otkazivanja nije dostupna korisnicima Enterprise ugovora sa državnom upravom SAD. Podržani su i drugi tipovi pretplata američke vlade, uključujući plaćanje po utrošku i CSP. Morate imati vlasnički pristup na Nalogu za rezervaciju da biste zamenili ili refundirali postojeću rezervaciju.

Sledeći koraci će vas voditi kroz postupak dovršavanja transakcije

1.Prijavite se na [Azure portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Izaberite rezervacije za koje želite da refundiranje bude refundiranje **i Exchange** 2.Izaberite VM proizvod koji želite da kupite i otkucajte količinu. Uverite se da je novi ukupni iznos kupovine veći od ukupnog iznosa povraćaja [Utvrdite pravu veličinu pre kupovine.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Pregledajte i dovršite transakciju

**Refundacija za rezervisanu instancu**

Da biste refundirali rezervaciju, idite na **Detalje rezervacije** i kliknite **Refundiraj**

**Proporcijalna refundacija:**

**Pro primeri refundacije i minimalnog zahteva za refundaciju i zamenu** Upfront rezervacij example:

- Kupujete jednogodišnji RI za 120 USD 1. januara
- 7. aprila želite da refundirate ili zamenite ovu rezervaciju
- Pošto je rezervacija aktivna 97 dana, dobićete nazad (1-97/365) * 120 USD. (tj. 88,1 USD). Trenutno nema kazne za refundaciju
- Ako menjate, vaša nova kupovina bi trebala biti veća od 88,1 USD
- Trenutno nema kazne za povraćaj sredstava

**Primer rezervacije plana naplate:**

- Kupujete jednogodišnji RI za 10 dolara mesečno
- 7. aprila želite da refundirate ili zamenite ovu rezervaciju
- Pošto se poslednja uplata dogodila 7 dana, dobićete nazad (1-7/31) * 10 USD. (tj. 7,74 USD)
- Buduće otkazane uplate iznose 80 USD. Trenutno nema kazne za refundaciju
- Ovo otkazivanje oduzeće vam 87,74 USD sa ograničenja refundacije od 50.000 USD
- Ako menjate, ukupna vrednost vaše nova kupovine bi trebala biti veća od 87,74 USD

**Ne možete da vidite fakturu za poslednji period naplate**

Iz nekih mogućih razloga možda ne vidite fakturu:

- Imate mesečni iznos kredita sa pretplatom koju niste premašili ili imate besplatnu probnu pretplatu. Faktura se generiše samo kada oslanjate na novac
- To je manje od 30 dana od dana kada ste se pretplatio na Azure
- Faktura još nije generisana. Sačekajte do kraja perioda naplate
- Ako niste administrator naloga, starije fakture vam možda neće biti dostupne

**Preuzmite fakturu sa Azure portala (.pdf)**

- Izaberite pretplatu sa stranice ["Pretplate" na](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Azure portalu kao korisnik [sa pristupom fakturama](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Izaberite **fakture**
- Kliknite **na dugme Preuzmi** fakturu da biste prikazali kopiju PDF fakture. Ako piše **Nije dostupno**, pogledajte zašto ne vidim [fakturu za poslednji period naplate?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Primanje fakture putem e-pošte (.pdf)**

- Izaberite pretplatu sa [stranice Pretplate.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Izaberite stavku **"Fakture", a** zatim stavku "Pošalji mi fakturu e-poštom"
- Kliknite **na dugme daj sa sažetku** i prihvatite uslove. Za svaku pretplatu morate dati saklon za svaku pretplatu u čijoj ste

Na primer: Ako ne dobijete e-poruku nakon što ste pratili korake, uverite se da je vaša e-adresa ispravna u željenim opcijama komunikacije [na profilu](https://account.windowsazure.com/profile)

**Preuzmite podatke o korišćenje sa Azure portala**

- Prijavite se u [Azure centar za](https://account.windowsazure.com/Subscriptions) naloge kao [administ za nalog](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Izaberite pretplatu za koju želite da imate informacije o fakturi i o korišćenjem
- Izaberite **istoriju naplate**
- Izaberite **stavku Prikaži trenutnu** izjavu da biste videli procenu troškova u trenutku kada je procena generisana
- Izaberite **stavku Preuzmi korišćenje** da biste preuzeli dnevne podatke o korišćenjeu kao CSV datoteku. Ako vidite dve dostupne verzije, preuzmite verziju 2

Druga pitanja: [Posetite rezervisana dokumenta za instancu](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Preporučeni dokumenti**

- [Osnove naplate](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje primene rezervisanog popusta na instancu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Preuzimanje ili prikaz fakture za naplatu za Azure i dnevnih podataka o korišćenjem](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje primene rezervisanog popusta na instancu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervisane korišćenje instance za pretplatu na Pay-As-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervisane korišćenje instance za unošenje u Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows softverskih troškova koji nisu uključeni u rezervisane instance](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervisane instance u programu za centralnu Dobavljač rešenja u oblaku partneru (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)