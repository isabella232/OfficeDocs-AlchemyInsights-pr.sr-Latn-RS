---
title: Problem pri ponovnom podešavanju lozinke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696276"
---
# <a name="problems-resetting-password"></a>Problemi pri ponovnom podešavanju lozinke

Slede neki od problema sa kojima možete da se suoиite prilikom ponovnog podešavanja lozinke i mogućih rešenja:

**Imam problem sa poništavanju lozinke koje nisu obuhvaćene drugim kategorijama**

- Uverite se da ste ovlašćeni za poništavanje lozinki. Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke. Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.
- Uverite se da razumete zahteve licenciranja:
    - Morate imati bar jednu licencu dodeljenu u organizaciji
        - Samo oblaci korisnici – bilo koji Office 365 (O365) plaćeni MJ ili Azure AD Basic
        - Cloud i/ili lokalno korisnici – Azure AD Premium P1 ili P2, Enterprise mobilnost + Security (EMS) ili bezbedno preduzeće (SPE)
        - Da biste pročitali više o zahtevima licenciranja pogledajte [zahteve za licenciranje članaka za Azure AD samouslužno poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**Imam problema sa ispitivanjem smernica za poništavanje lozinke koju sam podesio**

- Nedavno zatvorene smernice mogu potrajati nekoliko minuta radi replikaciju u svim centrima podataka i krajnjim tačkama. Fizički razdaljina iz centra za podatke će takođe uticati na primenu primene promena.
- Testiranje sa krajnjim korisnikom, ne administratorom i pilotu sa malim skupom korisnika. Smernice podešene na Azure portovi primenjuju se samo na krajnje korisnike, ne na administratore. Microsoft obavezuje podrazumevane smernice za poništavanje lozinke sa dve kapije za bilo koju Azure administratorsku ulogu (primer: globalni administrator, HelpDesk administrator, administrator lozinki itd.)
    - Saznajte više o [smernicama za administratore](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**Želim da pokrenem poništavanje lozinke, ali ne želim da moji korisnici registruju dodatne bezbednosne informacije**

Unapred popunjavate podatke za korisnike tako da ne moraju! -Kao administrator možete da postavite svojstva telefona i e-pošte za korisnike pre nego što izazovete poništavanje lozinki na organizaciju. To možete da uradite koristeći API, PowerShell ili Azure AD Connect. Više informacija potražite u člancima:
- [Primena početne vrednosti poništavanja bez potrebe korisnika da se registruju](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Koje podatke koristi poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dugme "poništi lozinku" je premačeno**

Nemate dozvolu da poništite lozinke ovog korisnika. Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke. Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.

**Ne vidim nož za poništavanje lozinke**

Nemate dozvolu da poništite lozinke. Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke. Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.

**Ne mogu da vidim lokalnu oљtricu za integraciju u polju za poništavanje lozinke**

- Oљtrica lokalno integracije se pojavljuje samo u hibridne okruženja – što znači da koristite ispravnu lozinku za manipulisanje lozinkama korisnika.
- Ne vidite ovaj nož ako:
    - Ne koristite ponovno upisivanje lozinki
    - Postoji problem sa instalacijom/povezivanjem lozinke za poništavanje lozinki
    - Postoji problem sa instalacijom/povezivanjem Azure AD Connect
    - Više koraka za rešavanje problema sa lozinkama pri vraćanju lozinki potražite u odeljku [Rešavanje problema sa lozinkom](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support) ispravkom

**Ne znam kako da poništim lozinku korisnika**

1. Prijavite se na Azure portal kao odgovarajući administrator.
1. Idite na Blade za korisnike i grupe, izaberite stavku **Svi korisnici**.
1. Izaberite korisnika sa liste.
1. Za izabranog korisnika, izaberite stavku **Pregled**, a zatim na komandnoj traci kliknite na dugme **Poništi lozinku**.
1. Izvršite uputstva na ekranu.
    - Samo resetima koji se izvršavaju putem Azure portala podržavaju ponovno upisivanje lozinki.

**Resetovao sam lozinku lokalnog korisnika sa Office 365 portala administracije ili Office 365 mobilnog aplikacije, ali korisnik i dalje ne može da se prijavi**

Povratni lozinku nije podržan na ovom portalu. Ponovo poništite lozinku korisnika u Azure portalu – portal.azure.com

