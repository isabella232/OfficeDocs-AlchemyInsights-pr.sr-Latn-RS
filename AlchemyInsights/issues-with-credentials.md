---
title: Problemi sa akreditima
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986833"
---
# <a name="issues-with-credentials"></a>Problemi sa akreditima

Microsoft platforma za identitete i [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) klijentski tok akreditiva opisuje kako da se program prikazuje direktno u odnosu na tok odobravanja Akreditiva klijenta OAuth 2.0.

**Kako da upravljam lozinkom ili akreditima za certifikat aplikacije?**

U Azure CLI aplikaciji možete da koristite [akrediitivi aplikacije Az ad da](https://docs.microsoft.com/cli/azure/ad/app/credential) biste izbrisali, naveli ili poništili lozinku aplikacije ili akredicije certifikata.

**Kako korisnici poništavaju lozinke?**

Korisnici treba da se [registruju za samouslužno poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) da bi mogli da ponište lozinke. Kada se korisnik registruje, može da prati uputstva iz ovog članka da bi poništio lozinku: Poništite lozinku na poslu [ili u školi.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)

**Kako korisnici menjaju lozinke?**

Korisnici mogu da prate korake u ovom članku kako bi promenili lozinke: [Kako da promene lozinku.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
Takođe mogu da [upravljaju lozinkama aplikacije za verifikaciju u dva koraka.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**Moj korisnik dobija grešku prilikom promene ili poništavanja lozinke**

Ova veza pruža informacije o uobičajenim problemima koji mogu nastati kada korisnik pokuša da poništi lozinku: Uobičajeni problemi [i njihova rešenja](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Imam problem sa poništavanje lozinke korisnika**

- Uverite se da ste ovlašćeni za poništavanje lozinki. *Samo globalni, lozinka i administratori korisnika mogu da ponište korisničke lozinke.* Globalni administratori takođe mogu da ponište lozinke drugih privilegovanih administratora.

- Uverite se da ste razumeli zahteve za licenciranje:

  - Morate imati barem jednu licencu dodeljenu u organizaciji:
    - **Samo korisnici u oblaku** – Svi Office 365 (O365) plaćeni SKU ili Azure AD Basic
    - **Oblak i/ili** korisnici – Azure AD Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure Productive Enterprise (SPE)
    - Da biste saznali više o zahtevima za licenciranje, pogledajte zahteve za licenciranje za samouslužno poništavanje lozinke za [Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Da biste poništili lozinku korisnika, pronađite korisnika u Azure AD. Zatim na bleju za pregled za tog korisnika kliknite na dugme "poništi lozinku".

**Dugme za poništavanje lozinke je zasićeno**

Niste ovlašćeni da **poništite** lozinke ovog korisnika. *Samo globalni, lozinka i administratori korisnika mogu da ponište korisničke lozinke.* Globalni administratori takođe mogu da ponište lozinke drugih privilegovanih administratora.

**Ne vidim blejd za poništavanje lozinke**

Niste ovlašćeni za poništavanje lozinki. *Samo globalni, lozinka i administratori korisnika mogu da ponište korisničke lozinke.* Globalni administratori takođe mogu da ponište lozinke drugih privilegovanih administratora.

**Ne vidim besmisleni blejd integracije u poništavanje lozinke**

- Blejd integracije se pojavljuje samo u hibridnim okruženjima – što znači da koristite pisanje lozinkom da biste manipulisali lozinkama korisnika.

- Ovaj blejd ne vidite ako:

  - Ne koristite pisanje lozinkom
  - Došlo je do problema sa instalacijom/povezivanjem za upisivanja lozinke
  - Postoji problem sa instalacijom/povezivanjem Azure AD Povezivanje
  - Za više koraka za rešavanje problema sa pisanjem lozinke, pogledajte rešavanje problema [sa pisanjem lozinke](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ne znam kako da poništim lozinku korisnika**

1. Prijavite se na Azure portal kao odgovarajući portal.
2. Idite na **blejd Korisnici i grupe** i izaberite stavku Svi **korisnici.**
3. Izaberite korisnika sa liste.
4. Za izabranog korisnika izaberite **stavku** Pregled , a zatim na komandnoj traci izaberite stavku Poništi **lozinku**.
5. Kliknite na dugme **Poništi lozinku** i pratite uputstva na ekranu.
    - Samo poništavanje izvršeno putem upisa **lozinke za Azure portal.**

**Poništavam lozinku korisnika u Office 365 administracija portalu ili Office 365 aplikaciji za mobilne uređaje, ali korisnik i dalje ne može da se prijavi**

Pisanje lozinkom nije podržano na ovom portalu. Ponovo poništite lozinku korisnika na Azure portalu.
