---
title: Problemi sa akreditivima
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
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063686"
---
# <a name="issues-with-credentials"></a>Problemi sa akreditivima

[Microsoft Platform identiteta i oauth 2,0 pristup akreditivima klijenta](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisuje kako se programira direktno sa oauth 2,0 akreditivima klijenata.

**Kako da upravljam lozinkom aplikacije ili akreditivima certifikata?**

U Azure CLI možete da koristite akreditiv [ad App App](https://docs.microsoft.com/cli/azure/ad/app/credential) za brisanje, listu ili resetovanje lozinke aplikacije ili akreditiva certifikata.

**Kako moji korisnici mogu da resetuju lozinke?**

Korisnici treba da se [registruju za samouslužno poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) pre nego što mogu da resetuju lozinke. Kada se korisnik registruje, oni mogu da slede uputstva iz ovog članka da bi poništili svoju lozinku: [poništili lozinku za posao ili školu](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).

**Kako korisnici menjaju lozinke?**

Korisnici mogu da slede korake iz ovog članka da bi promenili lozinke: [Kako da promenite lozinku](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).
Takođe mogu da [upravljaju lozinkama za aplikacije iz dva koraka](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).

**Moj korisnik dobija grešku prilikom promene ili ponovnog podešavanja lozinke**

Ova karika će pružiti informacije o uobičajenim problemima koji mogu da se pojave kada korisnik pokušava da poništi lozinku: [uobičajeni problemi i rešenja](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**Imam problem sa ponovnim postavljanjem lozinke korisnika**

- Proverite da li ste ovlašćeni za poništavanje lozinki. *Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.* Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.

- Uverite se da ste razumeli zahteve licenciranja:

  - Morate imati bar jednu licencu dodeljenu u organizaciji:
    - **Samo oblaci korisnici** – bilo koji Office 365 (O365) plaćeni MJ ili AZURE AD Basic
    - **Cloud i/ili lokalno korisnici** – AZURE AD Premium P1 ili P2, Enterprise mobilnost + Security (Ems) ili bezbedno preduzeće (SPE)
    - Da biste saznali više o zahtevima licenciranja, pogledajte članak [licenciranje zahteva za pretraživanje lozinke za Azure AD samouslužno](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- Da biste poništili lozinku korisnika, pronađite korisnika u usluzi Azure AD. Zatim, na oštrici za taj korisnik kliknite na dugme "poništi lozinku".

**Dugme "poništi lozinku" je premačeno**

Nemate dozvolu da poništite lozinke **ovog** korisnika. *Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.* Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.

**Ne vidim nož za poništavanje lozinke**

Nemate dozvolu da poništite lozinke. *Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.* Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.

**Ne mogu da vidim lokalnu oљtricu za integraciju u polju za poništavanje lozinke**

- Oљtrica lokalno integracije se pojavljuje samo u hibridne okruženja – što znači da koristite ispravnu lozinku za manipulisanje lozinkama korisnika.

- Ne vidite ovaj nož ako:

  - Ne koristite ponovno upisivanje lozinki
  - Postoji problem sa instalacijom/povezivanjem lozinke za poništavanje lozinki
  - Postoji problem sa instalacijom/povezivanjem Azure AD Connect
  - Više koraka za rešavanje problema sa lozinkama pri vraćanju lozinki potražite u članku [Rešavanje problema sa lozinkom ponovno upisivanje](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**Ne znam kako da poništim lozinku korisnika**

1. Prijavite se na Azure portal kao odgovarajući administrator.
2. Idite na Blade za **korisnike i grupe** , izaberite stavku **Svi korisnici**.
3. Izaberite korisnika sa liste.
4. Za izabranog korisnika, izaberite stavku **Pregled**, a zatim na komandnoj traci izaberite stavku **Poništi lozinku**.
5. Kliknite na dugme **Poništi lozinku** i uradite uputstva na ekranu.
    - Samo resetima koji se izvršavaju putem **Azure portala** podržavaju ponovno upisivanje lozinki.

**Resetovao sam lozinku lokalnog korisnika sa Office 365 portala administracije ili Office 365 mobilnog aplikacije, ali korisnik i dalje ne može da se prijavi**

Povratni lozinku nije podržan na ovom portalu. Ponovo uspostavite lozinku korisnika na Azure portalu.
