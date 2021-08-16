---
title: Problem sa poništavanje lozinke
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
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039980"
---
# <a name="problems-resetting-password"></a>Problemi sa poništavanje lozinke

U nastavku slede neki od problema sa kojima se možete suočiti prilikom poništavanja lozinke i do mogućih rešenja:

**Imam problem sa poništavanje lozinke koje nije pokriveno u drugim kategorijama**

- Uverite se da ste ovlašćeni za poništavanje lozinki. Samo globalni, lozinka i administratori korisnika mogu da ponište korisničke lozinke. Globalni administratori takođe mogu da ponište lozinke drugih privilegovanih administratora.
- Uverite se da razumete zahteve za licenciranje:
    - Morate imati dodeljenu najmanje jednu licencu u organizaciji
        - Samo korisnici u oblaku – Svi Office 365 (O365) plaćeni SKU ili Azure AD Basic
        - Oblak i/ili korisnici – Azure AD Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure Productive Enterprise (SPE)
        - Da biste pročitali više o zahtevima za licenciranje, pogledajte članak Zahtevi licenciranja za samouslužno poništavanje lozinke za [Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**Imam problema sa testiranjem smernica za poništavanje lozinke koje postavim**

- Nedavno primenjene smernice može potrajati nekoliko minuta da se replicira u svim centrima podataka i krajnjim tačkama. Fizička udaljenost od centra podataka utiče i na brzinu primene promena.
- Testirajte sa krajnjim korisnikom, ne sa administratorom i isprobajte ga sa malim skupom korisnika. Smernice konfigurisane na Azure portalu važe SAMO za krajnje korisnike, a ne za administratore. Microsoft nalaže jake smernice za poništavanje lozinke sa dva mrežna prolaza za svaku ulogu administratora usluge Azure (primer: Globalni administrator, administrator tehničke podrške, administrator lozinke itd.)
    - Saznajte više [o smernicama za administratore.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Želim da primenim poništavanje lozinke, ali ne želim da korisnici registruju dodatne bezbednosne informacije**

Unapred popunite podatke za korisnike kako oni to ne bi morali! – Kao administrator možete da podesite svojstva telefona i e-pošte za korisnike pre nego što u vašoj organizaciji postavite poništavanje lozinke. To možete da uradite pomoću API-ja, programa PowerShell ili Azure AD Povezivanje. Više informacija potražite ovde:
- [Primena poništavanja lozinke bez korisnika koji moraju da se registruju](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Koje podatke poništavanje lozinke koristi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dugme za poništavanje lozinke je zasićeno**

Niste ovlašćeni da poništite lozinke ovog korisnika. Samo globalni, lozinka i administratori korisnika mogu da ponište korisničke lozinke. Globalni administratori takođe mogu da ponište lozinke drugih privilegovanih administratora.

**Ne vidim blejd za poništavanje lozinke**

Niste ovlašćeni za poništavanje lozinki. Samo globalni, lozinka i administratori korisnika mogu da ponište korisničke lozinke. Globalni administratori takođe mogu da ponište lozinke drugih privilegovanih administratora.

**Ne vidim besmisleni blejd integracije u poništavanje lozinke**

- Blejd integracije se pojavljuje samo u hibridnim okruženjima – što znači da koristite pisanje lozinkom da biste manipulisali lozinkama korisnika.
- Ovaj blejd ne vidite ako:
    - Ne koristite pisanje lozinkom
    - Došlo je do problema sa instalacijom/povezivanjem za upisivanja lozinke
    - Postoji problem sa instalacijom/povezivanjem Azure AD Povezivanje
    - Za više koraka za rešavanje problema sa pisanjem lozinke, pogledajte odeljak Rešavanje problema [sa pisanjem lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ne znam kako da poništim lozinku korisnika**

1. Prijavite se na Azure portal kao odgovarajući portal.
1. Idite na blejd Korisnici i grupe i izaberite stavku **Svi korisnici.**
1. Izaberite korisnika sa liste.
1. Za izabranog korisnika izaberite **stavku** Pregled , a zatim na komandnoj traci izaberite stavku Poništi **lozinku.**
1. Sledite uputstva na ekranu.
    - Samo poništavanje izvršeno putem upisa lozinke za Azure portal.

**Poništavam lozinku korisnika u Office 365 administracija portalu ili Office 365 aplikaciji za mobilne uređaje, ali korisnik i dalje ne može da se prijavi**

Pisanje lozinkom nije podržano na ovom portalu. Ponovo poništite lozinku korisnika na Azure portalu – portal.azure.com

