---
title: Zašto dugme "Dodaj budžet" bude omogućeno za mene?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807668"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Zašto dugme "Dodaj budžet" bude omogućeno za mene?

Da biste kreirali budžet, potrebna vam je jedna od sledećih dozvola:

- Grupa za upravljanje, pretplata, opsezi grupe resursa
- Saradnik za upravljanje troškovima
- La
- Donator
- Samo za klijente klijenta: prijavljivanje, odeljenje, opsezi naloga
- Administrator upisivanja (podešava budžet na opsegu upisivanja)
- Administrator odseka (Podesi budžet na opsegu odseka)
- Vlasnik naloga (Podesi budžet na opsegu naloga)
- Samo savremeni ugovor o klijentu: nalog naplate, profil naplate, opsege odeljka fakture
- Azure kreator pretplate

**Kreirao sam budžet kada je trošak trenutnog meseca već bio iznad budžeta. Zašto nisam primio obaveštenje?**  
Ako ste već premašili navedeni cenzus cost kada kreirate budžet koji upozorenje neće biti ispaljeno. Kada počne novi ciklus, ako prekršite cenzus, upozorenje će se zapaliti.

**Kada treba da očekujem da ću dobiti obaveštenje nakon što premašim određeno ograničenje budžetskog obaveštenja o budžetu?**  
Budžeti se procenjuju na svakih 4 sata. Potrebno je minimalno 8 časova da bi se podaci o korišćenju budžetom dostigli sistem. S obzirom na ovo, obaveštenja će možda potrajati dok ne prekoračite cenzus od 12 časova.

**Zašto se dugme "Datum početka" Onemogući kada izaberem mesečni period ponovnog fakturisanja?**  
Budžeti su poravnati sa trenutnim mesečnim kalendarima ili trenutnim periodom naplate (u slučaju kada je potvrđen izbor u mesecu fakturisanja). Zbog toga ćemo unapred popuniti ovu vrednost za vas.

**Zašto ne vidim grafikon troškova prilikom iskustva prilikom kreiranja budžeta?**  
Treba nam minimum 2 meseca troškova podataka pre nego što možemo da ukaћemo grafikon kako bi vam pomogao pri kreiranju budžeta.

**Zašto ne mogu da podesim budžet sa pretplatom koju sam upravo kreirao?**  
Nakon kreiranja pretplate, podaci treba 24-48 sati da se obrade pre nego što postavite budžet protiv njega.

**Resursi za budžet budžeta**

- [BUDŽETI API V12](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): pruža operacije za kreiranje i ažuriranje budžeta. Pomoću API-ja budžeta možete da podesite cenzus budžeta i konfigurišete više obaveštenja da biste pucali dok ste priљli tom pragu. Obaveštenja mogu da aktiviraju e-poruku ili Azure radnju za obavljanje automatizacije. Napomena: filtriranje za ovaj API ne poravnava sa API-om filtriranja/dimenzija.
- [BUDŽETI API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Kreirajte budžete sa većim sposobnostima filtriranja troškova od V1. Filtriranje se poravnava sa ugovorom korišćenim u upitu i API-Jima. Ovo je preporučeni budžet API za kretanje dalje.
- [Dimenzije](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): pruža operacija da biste dobili podržane dimenzije za upotrebu ispod raznih opsega. Pomoću API dimenzije možete da preuzmete listu dimenzija koje mogu da se koriste kao ulaske za kreiranje upita pomoću API upita.
- [Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): pruža operacije da biste dobili agregirani trošak i podatke o korišćenju na osnovu upita koji snabdevas. Pomoću API upita možete da navedete željeno filtriranje, sortiranje i grupisanje u svim dostupnim dimenzijama (kojima se pristupa iz upite dimenzije).

**Predviđene troškove**

**Zašto ne vidim predviđanja za moje troškove u analizi troška?**  
Postoji više razloga zbog kojih možda postoji projekcija predviđanja u okviru analiza troškova, a neka od njih su sledeća:

1. Ako je trošak podataka star manje od 10 dana, grafikon predviđanja se neće učitavati. Model zahteva najmanje 10 dana nedavnih podataka o troškovima za tačne projekcije
2. Ako ste izabrali istorijske datume, grafikon predviđanja neće biti vidljiv. Izaberite opseg datuma sa budućim datumima za predviđenu opciju
3. Ako vaš nalog ima više valuta, grafikon predviđanja će samo projektovati troškove za ' sve troškove u USD '

**Zašto se predviđanje ne menja kada promenim resurse?**  
Model predviđanja zahteva nekoliko dana za nalog za promene na nalogu i ne pravi momentalne projekcije na osnovu promene resursa  
Za veće korake povećanja ili smanjenja resursa, model će potrajati malo duže da bi se prilagodio ovim promenama u nalogu za anomalije

**Zašto se moje predviđanje povećava kada rezervišem kupovinu ili Marketplace?**  
Model predviđanja smatra da su to "Stvarni troškovi" i da se ne računa za upotrebu i nabavku zasebno. Za jednokratnu kupovinu, model će smanjiti projekcije posle 10 dana da bi se uključilo nagli porast troškova

**Želim da vidim prognoze za jednu dimenziju (npr. Centimetra**  
Prognoza trenutno podržava ukupne projekcije troškova i ne za pojedinačne Merete. Stoga, kada je "grupisana po" dimenziji, projekcije će biti za ukupan broj svih stavki u dimenziji

**Preporučeni dokumenti**

- [Šta je to Azure upravljanje troškovima?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najbolje prakse Azure upravljanja troškovima](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Analizirajte troškove i potrošnju](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Istražite i analizirajte troškove pomoću analize troška](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure upravljanje troškovima: cenovnik](https://azure.microsoft.com/services/cost-management/#pricing)
- [Pregled troškova u analizi troška](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Uputstvo za video: kreiranje budžeta na Azure portalu](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Preduslovi za pregled i prilagođavanje budžete](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Kreiranje budžeta i upravljanje njima](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Konfigurisanje automatizacije sa Azure akcionim grupama i budžetom API-Jima](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Koristite obaveštenja o troškovima da biste nadgledali upotrebu i potrošnju](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Najbolje prakse upravljanja troškovima](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Uputstvo za uputstvo**

- [Kreiranje budžeta na Azure portalu](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Upravljanje troškovima uz API i akcione grupe](https://go.microsoft.com/fwlink/?linkid=2147038)