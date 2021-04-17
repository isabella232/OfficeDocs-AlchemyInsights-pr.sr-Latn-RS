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
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820336"
---
# <a name="billing-for-reserved-instance-purchase"></a>Naplata za kupovinu rezervisane instance

Rezervisana kupovina instanci se naplaćuje načinom plaćanja koji je vezan za pretplatu koju ste izabrali u vreme kupovine. Tip pretplate mora da bude ugovor sa preduzećem (broj ponude: MS-AZR-0017P), Pay-As-You-Go (broj ponude: MS-AZR-0003P), Microsoft korisnički ugovor ili CSP.

- Za pretplatu na preduzeća, troškovi se oduzimaju iz salda monetarne obaveze upisa ili se naplaćuju kao prekomerno korišćenje
- Za pretplatu na Pay-As-Go, troškovi se naplaćuju na kreditnoj kartici ili načinu plaćanja po fakturi za pretplatu

**Otkazivanje rezervacije**

- **Samouslužno:** Rezervisanu instancu možete sami da otkažete ili zamenite [koristeći Azure portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Izaberite rezervaciju i kliknite na refundiranje ili zamenu. Imajte u toga da morate imati pristup vlasnika u porudžbini rezervacije da biste razmenjili ili refundisali. Pristup samo Rezervaciji ne može da vam dozvoli da nastavite sa refundom ili zamenom. Tražite od vlasnika porudžbine rezervacije da vam da pristup porudžbini rezervacije
- **Exchange smernice:** Možete da zamenite rezervaciju za drugu rezervaciju istog tipa – za zamenu u **rezervaciji** ne postoje rezervacije. Ukupna obaveza uz novu rezervaciju trebalo bi da bude veća od zbira refundatornog iznosa rezervacije i budućih mesečnih rata (ako je primenljivo)
- **Smernice za refundator:** Zbir refundcije i otkazana buduća plaćanja ne mogu da premaše 50.000 USD u periodu od 12 meseci. Trenutno ne **naplaćujemo nijednu kasu** na refundcije, ali možemo da naplatimo buduće refundcije

**Izuzeci:** Samouslužna razmena i otkazivanje nisu dostupni za korisnike ugovora za državne uprave SAD

- **API /PS / CLI** podrška nije dostupna za otkazivanje i refundaciju samouslužnih zamena i [refundaciju za Azure rezervacije](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samouslužna razmena i otkazivanje nisu dostupni za klijente ugovora za državne uprave SAD. Podržani su i drugi tipovi pretplata za državne uprave SAD, uključujući Pay-As-You-Go i CSP

Saznajte više: [Kako se obrađuju](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) povratne i exchange transakcije Saznajte više: Smernice za Exchange i [refundacije](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Druga pitanja: Posetite [rezervisane](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support) dokumente instance

**Razmena postojeće rezervisane instance (samouslužno)**

Možete da zamenite rezervaciju za drugu rezervaciju istog tipa. Takođe možete da refundnete rezervaciju u iznosu od do 50.000 USD godišnje ako vam više nije potrebna. Samouslužna razmena i otkazivanje nisu dostupni za klijente ugovora za državne uprave SAD. Podržani su i drugi tipovi pretplata za državne uprave SAD, uključujući Pay-As-You-Go i CSP. Morate da imate pristup vlasnika u porudžbini rezervacije da biste razmenjili ili refundisali postojeću rezervaciju.

Sledeći koraci će vas voditi kroz proceduru za dovršenje transakcije

1.Prijavite se na [Azure portal.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Izaberite rezervacije za koje želite da refundiranje bude refundiranje i izaberite **stavku Exchange** 2.Izaberite VM proizvod koji želite da kupite i otkucajte količinu. Uverite se da je novi ukupni iznos kupovine veći od ukupnog iznosa povraćaja [Utvrdite pravu veličinu pre kupovine.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.Pregledajte i dovršite transakciju

**Refundirana instanca za rezervisanu instancu**

Da biste refundisali rezervaciju, idite na stavku **Detalji rezervacije i** izaberite **stavku Refundjanje**

**Ocenjena refundirana refundska zaliha:**

**Primeri proporcije i minimalnog zahteva za refundaciju i zamenu** Upfront rezervacij example:

- Kupujete jednogodišnji period RIJA za 120 USD 1. januara
- Želite da refundelite ili zamenite ovu rezervaciju 7. aprila
- Pošto se rezervacija živi 97 dana, dobijate (1-97/365) * 120 USD nazad. (iznosi 88,1 USD). Trenutno ne postoji zasniva se na refundacijama
- Ako je razmena veća od 88,1 USD, vaša nova kupovina bi trebalo da bude veća od 88,1 USD
- Trenutno ne postoji sažetije pretnje za refundcije

**Primer rezervacije plana naplate:**

- Kupujete jednogodišnji period RIJA za 10 USD mesečno
- Želite da refundelite ili zamenite ovu rezervaciju 7. aprila
- Od poslednjeg plaćanja u poslednjih 7 dana, dobijaćete (1–7/31) * 10 USD nazad. (naplaćeno 7,74 USD)
- Buduća otkazana plaćanja iznose 80 USD. Trenutno ne postoji zasniva se na refundacijama
- Ovo otkazivanje će oduziti 87,74 USD od ograničenja od 50.000 USD za refundaciju
- Ako je razmena veća od 87,74 USD, ukupna vrednost nove kupovine bi trebalo da bude veća od 87,74 USD

**Ne možete da vidite fakturu za poslednji period naplate**

Iz nekih mogućih razloga možda ne vidite fakturu:

- Imate mesečni iznos kredita sa pretplatom koju niste premašili ili imate besplatnu probnu pretplatu. Faktura se generiše samo kada oslanjate na novac
- To je manje od 30 dana od dana kada ste se pretplatio na Azure
- Faktura još nije generisana. Sačekajte do kraja perioda naplate
- Ako niste administrator naloga, starije fakture vam možda neće biti dostupne

**Preuzimanje fakture sa Azure portala (.pdf)**

- Izaberite pretplatu sa stranice ["Pretplate" na](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Azure portalu kao korisnik [sa pristupom fakturama](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Izaberite **fakture**
- Kliknite **na dugme Preuzmi** fakturu da biste prikazali kopiju PDF fakture. Ako piše **Nije dostupno**, pogledajte zašto ne vidim [fakturu za poslednji period naplate?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Prijem fakture putem e-pošte (.pdf)**

- Izaberite pretplatu sa [stranice Pretplate.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) Izaberite stavku **"Fakture", a** zatim stavku "Pošalji mi fakturu e-poštom"
- Kliknite **na dugme daj sa sažetku** i prihvatite uslove. Za svaku pretplatu morate dati saklon za svaku pretplatu u čijoj ste

Na primer: Ako ne dobijete e-poruku nakon što ste pratili korake, uverite se da je vaša e-adresa ispravna u željenim opcijama komunikacije [na profilu](https://account.windowsazure.com/profile)

**Preuzmite podatke o korišćenje sa Azure portala**

- Prijavite se u [Azure centar za](https://account.windowsazure.com/Subscriptions) naloge kao [administ za nalog](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Izaberite pretplatu za koju želite da imate informacije o fakturi i o korišćenjem
- Izaberite **istoriju naplate**
- Izaberite **stavku Prikaži trenutnu** izjavu da biste videli procenu troškova u trenutku kada je procena generisana
- Izaberite **stavku Preuzmi korišćenje** da biste preuzeli dnevne podatke o korišćenjeu kao CSV datoteku. Ako vidite dve dostupne verzije, preuzmite verziju 2

Druga pitanja: [Posetite rezervisane dokumente sa instancama](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Preporučeni dokumenti**

- [Osnove naplate](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje primene rezervisanog popusta na instancu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Preuzimanje ili prikaz fakture za naplatu za Azure i dnevnih podataka o korišćenjem](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje primene rezervisanog popusta na instancu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervisane korišćenje instance za pretplatu na Pay-As-Go](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervisane korišćenje instance za unošenje u Enterprise](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Troškovi Windows softvera nisu obuhvaćeni rezervisanim instancama](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervisane instance u programu Partner Central Cloud Solution Provider (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)