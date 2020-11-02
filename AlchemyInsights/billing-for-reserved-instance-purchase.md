---
title: Naplate za rezervisanu instancu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823168"
---
# <a name="billing-for-reserved-instance-purchase"></a>Naplate za rezervisanu instancu

Kupovina rezervisane instance je naplaćena za način plaćanja vezan za pretplatu koju ste izabrali u vreme kupovine. Tip pretplate mora da bude poslovni sporazum (broj ponude: MS-AZR-0017P), Pay-as-go (ponuda broj: MS-AZR-0003P), Microsoft ugovor ili CSP.

- Za pretplatu na Enterprise, troškovi se odbijaju od salda za monetarnu obavezu vezanosti za prijavljivanje ili naplaćuju u svojstvu
- Za pretplatu na karticu za plaćanje, troškovi se naplaćuju na kartici uplata ili faktura plaćanja za pretplatu

**Otkazivanje rezervata**

- **Samouusluga:** Rezervisanu instancu možete da otkažete ili da je razmenjujete pomoću [Azure portala](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izaberite rezervaciju i kliknite na povraćaj ili Exchange. Imajte u vidu da morate da imate pristup vlasniku u nalogu za rezervaciju da biste razmenili ili vratili povraćaj. Pristup samo rezervatu vam neće dozvoliti da nastavite sa povraćajem i Exchange serverom. Zamolite vlasnika naloga za rezervacije da vam pruži vlasniku pristup nalogu rezervacije
- **Smernice za Exchange:** Možete da zamenite rezervaciju za drugu rezervaciju iste vrste – nema **kazni** za razmenu rezervacija. Ukupna posvećenost novoj rezervaciji treba da bude veća od sume razmenjene uplate rezervacija i budućih mesečnih uplata (ako je primenljivo)
- **Smernice za povraćaj povraćaja:** Zbir refundacije i otkazanih budućih uplata ne mogu da premašuju $50.000 USD u 12-mjesečnom iskačućem prozoru. **Trenutno ne naplaćujemo nikakvu kaznu** za povraćaj novca, ali možemo da joj naplatimo za buduće povraćaj fondova

**Izuzeci:** Samouslužni Exchange i otkazivanje mogućnosti nisu dostupne za klijente AMERIČKOG vladinog sporazuma

- Podrška za **API/PS/CLI** nije dostupna za ukidanje [samouslužnog rada i povraćaj finansijskih usluga za Azure rezervacije](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Samouslužni Exchange i otkazivanje mogućnosti nisu dostupne za klijente AMERIČKOG vladinog sporazuma. Podržani su i drugi tipovi e-pošte koji uključuju Pay-as-go i CSP

Saznajte više: [Kako se vraćaju i Exchange transakcije obrade](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Saznajte više: [smernice za razmenu i povraćaj povraćaja](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) drugih pitanja: [posjecivi dokumenti na instanci](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Razmena postojeće rezervisane instance (samouslužno)**

Možete da zamenite rezervaciju za novu rezervaciju iste vrste. Rezervaciju možete da vratite i do $50.000 USD godišnje, ako vam više nije potrebna. Samouslužni Exchange i otkazivanje mogućnosti nisu dostupne za klijente AMERIČKOG vladinog sporazuma. Podržavaju se i drugi tipovi američkih vlada koji uključuju Pay-as-go i CSP. Da biste Exchange ili refundiranje postojeće rezervacije, morate imati pristup vlasniku.

Sledeći koraci će voditi proceduru za dovršavanje transakcije

1. prijavite se na [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade). Izaberite rezervacije koje želite da otkucate i kliknite na dugme **Exchange** 2. Izaberite tip proizvoda koji želite da kupite i otkucajte količinu. Uverite se da je nova ukupna vrednost kupovine veća od ukupnog zbira [određuje odgovarajuću veličinu pre kupovine](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).
3. pregledajte i dovršite transakciju

**Povraćaj sredstava za rezervisanu instancu**

Da biste vratili povraćaj rezervata, idite na **detalje** i izaberite stavku **povraćaj novca**

**Procijenjen povraćaj nivoa:**

**Primerci i primeri minimalnog zahteva za povraćaj i razmenu** Primer rezervata rezervacije:

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

**Nije moguće videti fakturu za poslednji period naplate**

Neki od mogućih razloga možda nećete videti fakturu:

- Imate mesečni iznos kredita sa pretplatom koju niste prešli ili imate besplatnu probnu verziju. Faktura se generiše samo kada duguješ novac
- To je manje od 30 dana od dana kada ste se pretplatili na Azure
- Faktura još uvek nije generisana. Čekanje do kraja perioda naplate
- Ako niste administrator naloga, starije fakture vam možda neće biti dostupne

**Preuzimanje fakture sa Azure portala (. pdf)**

- Izaberite pretplatu sa stranice " [pretplate](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) " u usluzi Azure kao [korisnik sa pristupom fakturama](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- Izbor **faktura**
- Izaberite stavku **Preuzmi fakturu** da biste PRIKAZALI kopiju PDF fakture. Ako piše " **nije dostupno** ", pogledajte [članak Zašto ne vidim fakturu za poslednji period naplate?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**Primite fakturu u e-poruci (. pdf)**

- Izaberite pretplatu sa stranice " [pretplate](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ". Izaberite stavku **fakture** i pošaljite e-poruku na fakturu
- Kliknite na dugme **odluči** i prihvatite uslove. Moraćete da se odlučite za svaku vašu pretplatu

Napomena: ako ne dobijete e-poruku nakon praćenja koraka, uverite se da je e-adresa tačna u [željenim postavkama komunikacije na profilu](https://account.windowsazure.com/profile)

**Preuzimanje podataka o korišćenju sa Azure portala**

- Prijavljivanje u [Centar Azure naloga](https://account.windowsazure.com/Subscriptions) kao [administrator naloga](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- Izaberite pretplatu za koju želite informacije o fakturi i korišćenju
- Izbor **istorije naplate**
- Izaberite stavku **Prikaži trenutnu izjavu** da biste videli procenu optužbi u vreme generisanja procene
- Izaberite stavku **Preuzimanje** da biste preuzeli svakodnevne podatke o korišćenju kao csv datoteku. Ako vidite dve dostupne verzije, preuzmite verziju 2

Druga pitanja: [posjetiti rezervisane dokumente instance](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Preporučeni dokumenti**

- [Osnove naplate](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje kako se zatvara popust na rezervisanu instancu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Preuzimanje ili prikazivanje Azure fakturisanja fakturisanja i dnevne upotrebe podataka o korišćenju](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje kako se zatvara popust na rezervisanu instancu](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervisane upotrebe instanci za pretplatu na koju se možete plaćati](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Razumevanje rezervisane upotrebe instance za primenu na poslovnom računaru](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows troškovi softvera nisu uključeni u rezervisane instance](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Rezervisane instance u programu provajdera za centralni plan partnerstva (CSP)](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)