---
title: Rešavanje problema sa grupama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "50714047"
---
# <a name="troubleshoot-group-issues"></a>Rešavanje problema sa grupama

**Moram da dodelim grupu za Azure reklamu**

Da biste grupi Azure Active Directory dodelili grupu Azure Active Directory (AD), obavite sledeće korake:

1. Kreirajte novu grupu – da biste kreirali novu grupu:

    Neko. Prijavite se u centar za Azure AD administracije sa privilegiranom administratorom uloge ili dozvolama za opšte administratore. 
    -. Izaberite Azure Active Directory > grupe > sve grupe > nova grupa. 
    trojku. Kreirajte grupu.

2. Dodelite ulogu grupi ili kada se grupa kreira.

    Neko. Da biste grupi dodelili ulogu u vreme kreiranja grupe, prebacivanje na opciju preklopnika Azure oglasa može biti dodeljeno grupi i Kreiranje grupe.
    -. Da biste dodelili ulogu grupi nakon kreiranja, pređite na karticu dodeljene uloge za novu grupu i dodelite joj ulogu.

**Treba da upravljam članstvom grupe koja je dodeljena usluzi Azure AD**

1. Da biste sprečili podizanje privilegija, podrazumevana vrednost samo administrator privilegija i globalni administrator mogu da izmene članstvo grupe koja je dodeljena ulozi. Međutim, oni mogu da izaberu da dodele vlasnika za takvu grupu i delegatu ovaj zadatak. Više informacija potražite u članku [Korišćenje grupa Cloud za upravljanje dodelama uloga u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).
2. Za uobičajena pitanja i savete za rešavanje problema za dodeljivanje uloga grupama u usluzi Azure AD, pogledajte odeljak [Rešavanje problema sa rasporedima u grupi Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).

**Dinamičke grupe**

1. Ako ne možete da pronađete ugrađene atribute korisnika, uverite se da se atribut nalazi na listi podržanih svojstava.
2. Ako tražite ugrađene atribute uređaja, uverite se da se atribut nalazi na listi atributa uređaja 
3. Pored ugrađenog atributa korisnika i uređaja, možete da koristite i [atribute proširenja](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties). Posle sinhronizacije atributa proširenja iz lokalnog Windows servera AD ili veze sa povezanom Sahas, atributi bi trebalo da budu vidljivi na padajućoj listi "Izrada pravila". Ime prilagođenog atributa može se pronaći u direktorijumu tako što će se upitati atribut korisnika pomoću programa PowerShell i tražiti ime atributa. To se može koristiti i prilikom izgradnje pravila u sintaksi pravila.
4. Uverite se da vaš stanar ima odgovarajuću licencu. Dinamičke grupe zahtevaju da zakupac ima licencu za Azure AD P1 Premium. Listi "Azure AD licenci" se može pristupiti [ovde](https://azure.microsoft.com/pricing/details/active-directory/). Preduzećima za mobilnost i pristup bezbednosnim dozvolama se može pristupiti [ovde](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).
5. Uverite se da je uloga korisnika koji kreira dinamičku grupu globalni administrator, Intune administrator, administrator grupe ili administrator korisnika.
6. Dozvolite da se grupa popunjava. U zavisnosti od veličine zakupca, grupi može biti potrebno do 24 časa za popunjavanje po prvi put ili posle promene pravila.
7. Više informacija potražite u članku [Kreiranje pravila zasnovanih na atributima za dinamičko članstvo u grupi](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).

**Treba da izbrišem grupu**

1. Grupe mogu da se brišu iz direktorijuma pomoću Remove-AzureADGroup cmdlet lokacije u Azure AD PowerShell modulu.
2. Pre nego što pokušate da izbrišete sinhronizovanu grupu u usluzi Azure AD, uverite se da ste izbrisali sve dodeljene licence da biste izbegli greške.
3. Više informacija o brisanju grupa potražite u članku [Brisanje grupe sa dodeljenom licencom](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).

**Treba da vratim izbrisanu grupu**

1. Ako je Office 365 grupa izbrisana, može da se vrati samo do 30 dana dok se ne pojavi trajno brisanje. Prilikom trajnog brisanja, grupa se više ne može obnoviti. Saznajte više o vraćanju grupa [ovde](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).
2. Ova funkcionalnost nije podržana za bezbednosne grupe i grupe za distribuciju.
3. Uverite se da ste ovlašćeni da biste vratili Office 365 grupu. Globalni administratori, administratori grupe, administratori korisničkog naloga, administratori usluge Intune, partneri tier1 ili tier2, a vlasnik grupe može da vrati grupu.
4. Kada se Dinamička grupa izbriše i vrati u prethodno stanje, ona se smatra novom grupom i ponovo se popunjava po pravilu. Ovaj proces može da potraje do 24 časa.
5. Više informacija o vraćanju izbrisane grupe potražite u članku [Vraćanje izbrisane Office 365 grupe u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Konfiguracija smernica za rok važenja grupe**

1. Ova funkcionalnost je podržana samo za Office 365 grupe i ne podržavaju ih bezbednosne grupe i grupe za distribuciju.
2. Konfigurisanje i korišćenje smernica za rok važenja za Office 365 grupe zahtevaju Azure AD Premium licencu.
3. Trenutno samo jedna smernica za rok važenja može da se podesi za Office 365 grupe na zakupcu.
4. Samo globalni administratori, administratori grupe, administratori korisnika i vlasnik grupe mogu da obnove grupu.
5. Ako je Office 365 grupa istekla, ona se briše i može da se vrati samo do 30 dana pre isteka trajnog brisanja. Prilikom trajnog brisanja, grupa se više ne može obnoviti. Saznajte više o vraćanju grupa [ovde](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Automatska obnova zasnovana na aktivnostima**

Korisničke aktivnosti iz sistema SharePoint, Outlook i timovi mogu da pokrenu grupnu automatsku obnovu grupe. Aktivnosti se provere na 35 dana pre isteka grupe. Ako postoji aktivnost tokom trenutnog ciklusa grupne trajanja grupe, grupa će se automatski obnoviti i neće se slati poruka e-poštom.

**Vreme obaveštavanja za istekle grupe**

1. Obaveštenja e-poštom se šalju u Office 365 vlasnike grupa 30 dana, 15 dana i 1 dan pre isteka grupe.
2. Kada prvi put podesite rok važenja, sve grupe koje su starije od intervala isteka su podešene na 35 dana dok ne istekne.
3. Datum isteka grupe izračunava se na osnovu datuma obnove grupe, ne zasnovane na datumu ažuriranja smernica. Ako se smernice za rok važenja ažuriraju, datum isteka se neće promeniti.
4. Više informacija potražite u članku [smernice za rok važenja grupe i e-poruke obnove](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) i [vraćanje izbrisane Office 365 grupe u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).

**Dozvola za kreiranje grupe**

Uverite se da ste ovlašćeni za kreiranje nove grupe. Globalni administratori mogu da onemoguće Kreiranje grupe na Azure portovu ili Access tabli. Možda će vam biti potreban administrator da biste kreirali novu grupu za vas ili da biste vam dali odgovarajuće dozvole.

1. [Kreiranje nove grupe i dodavanje članova na Azure portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Kreiranje grupa u programskom dodatku PowerShell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Onemogućavanje kreiranja grupa u programu PowerShell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Upravljanje ko može da kreira grupe u sistemu Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Onemogućavanje obaveštenja o usluzi Office 365 putem programskog dodatka PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD administrativne uloge](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Upravljanje dozvolama za kreiranje grupe**

1. Globalni administratori mogu da upravljaju dozvolama za kreiranje grupa za bezbednost ili Office 365 grupe kreirane na Azure portovi ili Access tabli, tako što će korisnici podešavanjem **korisnika da kreiraju bezbednosne grupe u Azure portali** ili **korisnici mogu da kreiraju Office 365 grupe u postavkama Azure portali** u **svim grupama > opšte (postavke)**.
2. Možete i da ograničite Kreiranje grupe da biste izabrali grupu korisnika ako imate licencu za Azure AD P1 Premium.

**Onemogućavanje obaveštenja o dobrodošlici za nove članove Office 365 grupe**

Obaveštenje o dobrodošlici koje se šalju korisnicima koji se dodaju u Office 365 grupe mogu da se sprečavaju tako što `UnifiedGroupWelcomeMessageEnabled` se podešava na **FALSE** u PowerShell. Saznajte više o ovoj podešavanju [ovde](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).













