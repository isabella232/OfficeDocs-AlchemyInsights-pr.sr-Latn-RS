---
title: Zašto je dugme "Dodaj budžet" onemogućeno za mene?
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
- "9003547"
- "6464"
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954693"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Zašto je dugme "Dodaj budžet" onemogućeno za mene?

Da biste kreirali budžet, potrebna vam je jedna od sledećih dozvola:

- Management Group, Subscription, Resource Group Scopes
- Saradnik u upravljanju troškovima
- Vlasnik
- Saradnik
- Samo klijenti iz preduzeća: Ugostite, Sektor, Opseza naloga
- Adminposte za unošenje (postavljen budžet u opsez uklonjanja)
- Adminitar sektora (podešen budžet u čijoj su dimenziji sektora)
- Vlasnik naloga (podešen budžet u čijoj su dimenziji naloga)
- Samo moderni korisnički ugovor: Nalog za naplatu, profil naplate, niski odeljka fakture
- Autor pretplate na Azure

**Napravio sam budžet kada je moj trošak za trenutni mesec već bio preko budžeta. Zašto nisam primio obaveštenje?**  
Ako ste već prekoračili dati prag troška kada napravite budžet koji se ne oslobada. Kada počne novi ciklus, ako kršite prag, upozorenje će se otpustiti.

**Kada treba da očekujem da primam obaveštenje nakon što premašim jednu od definisanih praga upozorenja o budžetu?**  
Budžeti se procenjuju svaka 4 časa. Potrebno je najmanje 8 sati da bi podaci o korišćenjem dostigli sistem budžeta. S obzirom na to, upozorenja mogu da traju i do 12 sati nakon što premašite ograničenje.

**Zašto je dugme "Datum početka" onemogućeno kada izaberem period poništavanja meseca ili meseca naplate?**  
Budžeti su usklađeni sa trenutnim kalendarski mesecom ili trenutnim periodom naplate (u slučaju kada je izabrana stavka Mesec naplate). Stoga ovu vrednost unapred popunimo za vas.

**Zašto ne vidim grafikon troškova u iskustvu sa kreiranjem budžeta?**  
Potrebno nam je najmanje 2 meseca troškova podataka da bismo mogli da kreiramo grafikon koji će vam pomoći pri kreiranju budžeta.

**Zašto ne mogu da podesim budžet za pretplatu koju sam upravo kreirao/rs?**  
Nakon kreiranja pretplate, obrada podataka od 24 do 48 sati pre postavljanja budžeta za njega.

**Budžet API resursa**

- [API budžeta v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Obezbeđuje operacije za pravljenje i ažuriranje budžeta. Pomoću API-ja budžeta možete da postavite prag budžeta i da konfigurišete više obaveštenja za upozorenja kada se približite tom pragu. Upozorenja mogu aktivirati e-poruku ili Azure grupu radnji radi automatizacije. Napomi: Filtriranje za ovaj API ne poravnava se sa API filtriranjem/dimenzijama upita.
- [API budžeta v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Kreirajte budžete sa većim mogućnostima filtriranja troškova od v1. Filtriranje je uravnoteženo sa ugovorom koji se koristi u AP-jem upita i dimenzija. Ovo je preporučeni API budžeta za korišćenje pomeranja unapred.
- [Dimenzije:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Obezbeđuje operacije za dobijanje podržanih dimenzija za korišćenje u okviru različitih oblasti. Pomoću API-ja dimenzija možete preuzeti listu dimenzija koje se mogu koristiti kao unosi za generisanje upita pomoću API-ja upita.
- [Upit:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Obezbeđuje operacije za dobijanje agregiranih troškova i podataka o korišćenjem na osnovu upita koji nabavljate. Pomoću API-ja upita možete da navedete željeno filtriranje, sortiranje i grupisanje po svim dostupnim dimenzijama (kojima se pristupa iz API-ja dimenzija).

**Prognozirani troškovi**

**Zašto ne vidim prognozme za svoje troškove u analizi troškova?**  
Postoji više razloga zbog kojih vam predviđanje možda nedostaje u analizi troškova, neki od njih su sledeći:

1. Ako su podaci o troškovima stariji od 10 dana, neće se učitati grafikon prognoza. Model zahteva najmanje 10 dana nedavnih troškova za precizne projekcije
2. Ako ste izabrali istorijske datume, grafikon prognoza neće biti vidljiv. Izaberite opseg datuma sa budućim datumima za prikazivanje grafikona sa prognozama
3. Ako vaš nalog ima više valuta, grafikon predviđanja će imati samo troškove projekta za "Sve troškove u USD"

**Zašto se prognoza ne menja kada napravim promene u resursima?**  
Model predviđanja zahteva par dana da bi se nalozile promene u nalogu i ne pravi trenutne projekcije na osnovu promene u resursima  
Za veće korake za povećanje ili smanjenje resursa, modelu će biti malo duže da se prilagodi ovim promenama kako bi uneo nepravilnosti

**Zašto se moje prognoza povećava kada napravim rezervaciju ili kupovinu na tržištu?**  
Model prognoza uzima u obzir "stvarni trošak" i ne uzima u obzir korišćenje i kupovinu posebno. Za jednodnevnu kupovinu model će smanjiti projekcije nakon 10 dana da bi se oglašavati iznenada povećavanje troškova

**Želim da vidim prognozione za jednu dimenziju (npr. metar)**  
Predviđanje trenutno podržava projekcije ukupnih troškova, a ne za pojedinačne metraže. Zato, kada se dimenzija "Grupiše po", projekcije će biti za ukupne vrednosti svih stavki u dimenziji

**Preporučeni dokumenti**

- [Šta je to upravljanje Azure troškovima?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najbolje prakse za upravljanje Azure troškovima](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analiziranje troškova i potrošnje](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Istraživanje i analiziranje troškova uz analizu troškova](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Upravljanje Azure troškovima: Cene](https://azure.microsoft.com/services/cost-management/#pricing)
- [Pregled troškova u analizi troškova](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Video uputstvo: Kreiranje budžeta na Azure portalu](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Preduslovi za prikazivanje i prilagođavanje budžeta](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Kreiranje budžeta i upravljanje budžetom](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurisanje automatizacije sa Azure grupama radnji i API-jem budžeta](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Korišćenje obaveštenja o troškovima za nadgledanje korišćenja i potrošnje](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najbolje prakse za upravljanje troškovima](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Video uputstva**

- [Kreiranje budžeta na Azure portalu](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Upravljanje troškovima uz API budžeta i grupe radnji](https://go.microsoft.com/fwlink/?linkid=2147038)