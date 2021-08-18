---
title: Pisanje lozinkom ne funkcioniše
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324937"
---
# <a name="password-writeback-is-not-working"></a>Pisanje lozinkom ne funkcioniše

**Imam problema sa konfigurisanje pisanjem lozinke**

- Pisanje lozinkom je premium funkcija.
- Uverite se da razumete zahteve za licenciranje:
  - Morate imati barem jednu licencu dodeljenu u organizaciji
  - **Samo korisnici u oblaku** – Svi Office 365 (O365) plaćeni SKU ili Azure AD Basic
  - **Oblak i/ili** korisnici – Azure AD Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure Productive Enterprise (SPE)
    - Da biste saznali više o zahtevima za licenciranje, pogledajte zahteve za licenciranje za samouslužno poništavanje lozinke za [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Imate bar jedan administratorski nalog i jedan probni korisnički nalog sa jednom od odgovarajućih licenci.
- Morate da povežete Azure AD Povezivanje emulator primarnog kontrolera domena da bi pisanje lozinke radilo. Azure AD Povezivanje možete da konfigurišete tako da koristi primarni kontroler domena tako što ćete kliknuti desnim tasterom miša na svojstva konektora za sinhronizaciju usluge Active Directory, a zatim izabrati konfiguriši particije  direktorijuma.  Odatle možete da  pogledate odeljak sa postavkama veze kontrolera domena i izaberite polje za potvrdu pod nazivom Samo koristite **željene kontrolere domena.**
    **Naznaka**:Ako željeni DC nije PDC emulator, Azure AD Povezivanje će i dalje kontaktirati PDC za upisivanje lozinki.
- Poništavanje lozinke je konfigurisano i omogućeno u vašem zakupca. Više informacija potražite u [temi Omogućavanje korisnicima da ponište svoje Azure AD lozinke.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Proverite da li je administratorski nalog koji se koristi za omogućavanje funkcije "Pisanje lozinke" administratorski nalog u oblaku (koji je kreiran u uslugi Azure AD, a ne za uslugu AD)
- Imate primenu usluge sa jednom šumom ili više šuma AD na kome su instalirani najnoviji servisni paketi Windows Server 2008 R2, Windows Server 2012 ili Windows Server 2012 R2 sa instaliranim najnovijim servisnim paketima
- Imate instaliranu alatku Azure AD Povezivanje i pripremili ste AD okruženje za sinhronizaciju sa oblakom. Pre nego što testirate pisanje lozinkom, uverite se da ste prvo dovršili kompletnu i uvoznu i kompletnu sinhronizaciju sa AD i Azure AD u Azure AD Povezivanje.
- Da biste saznali više, pogledajte kako da sinhronizujete [i kompletno uvezete u Azure AD Povezivanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Imam problem sa povezivanjem za pisanje lozinke**

1. Preuzmite i omogućite najnoviju verziju [usluge Azure AD Povezivanje](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracija zaštitnog zida: Azure AD Povezivanje alatki (1.1.443 i novijim) biće potreban odlazni **HTTPS** pristup:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Omogućavanje neisporučivanih veza da se traju najmanje 2–3 minuta

**I dalje imam problema sa pisanjem lozinki**

- Ako i dalje imate poteškoća, pokušajte da poremetite i ponovo omogućavate uslugu upisivanja lozinke u alatki Azure AD Povezivanje
- Da biste saznali više, pogledajte kako da onemogućite [i ponovo omogućite pisanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
