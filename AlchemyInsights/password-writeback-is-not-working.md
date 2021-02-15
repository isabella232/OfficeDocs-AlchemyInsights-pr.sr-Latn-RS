---
title: Vraćanje lozinki ne radi
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243521"
---
# <a name="password-writeback-is-not-working"></a>Vraćanje lozinki ne radi

**Imam problema sa konfigurisanjem sinhronizacijom lozinki**

- Ponovno upisivanje lozinki je Premium funkcija.
- Uverite se da razumete zahteve licenciranja:
  - Morate imati bar jednu licencu dodeljenu u organizaciji
  - **Samo oblaci korisnici** – bilo koji Office 365 (O365) plaćeni MJ ili AZURE AD Basic
  - **Cloud i/ili lokalno korisnici** – AZURE AD Premium P1 ili P2, Enterprise mobilnost + Security (Ems) ili bezbedno preduzeće (SPE)
    - Da biste saznali više o zahtevima licenciranja, pogledajte članak [licenciranje zahteva za Azure AD samouslužno poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Imate najmanje jedan administratorski nalog i jedan probni korisnički nalog sa jednom od odgovarajućih licenci.
- Morate da povežete Azure AD se poveže sa glavnim Emulatorom kontrolora domena za upisivanje lozinki na posao. Možete da konfigurišete Azure AD Connect da biste koristili primarni kontroler domena tako što ćete kliknuti desnim tasterom miša na **Svojstva** konektora za sinhronizaciju aktivnog direktorijuma, a zatim izabrati stavku **Podešavanje Particija direktorijuma**. Odatle potražite odeljak **Postavke veze sa kontrolerom domena** i potvrdite izbor u polju za potvrdu pod naslovom **samo koristite željene kontrolore domena**.
  > [!NOTE]
  > Ako centar za željeni centar nije PDC Emulator, Azure AD Connect i dalje dostižu PDC-u za ponovno upisivanje lozinki.
- Poništavanje lozinke je podešeno i omogućeno u vašem zakupcu. Više informacija potražite u članku [Omogućavanje korisnicima da resetuju svoje Azure oglase lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).
- Uverite se da je administratorski nalog koji se koristi za omogućavanje ispravnosti lozinki administratorski nalog (kreiran u okviru Azure AD nije lokalni AD)
- Imate jedan ili više šuma OGLAŠAVANJE na lokalnom sajtu koji radi pod operativnim sistemom Windows Server 2008 R2, Windows Server 2012 ili Windows Server 2012 R2 sa instaliranim najsavremenijim servisnim paketima
- Imate instaliranu alatku Azure AD Connect i pripremili ste reklamu za sinhronizaciju u oblaku. Pre nego što testirate poništavanje lozinki, uverite se da ste prvi put dovršili sa sinhronizacijom kompletne i potpune sinhronizacije iz AD i Azure AD u usluzi Azure AD Connect.
- Da biste saznali više, pogledajte članak kako se radi [potpuna sinhronizacija i kompletan uvoz u usluzi Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Imam problem sa mogućnošću povezivanja lozinki**

1. Preuzmite i omogućite najnoviju verziju usluge [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Konfiguracija zaštitnog zida: alatka Azure AD Connect (1.1.443 i iznad) Trebaće im **HTTPS** pristup na:
    - passwordreset.microsoftonline.com
    - servicebus. Windows. mreže
3. Omogući da veza sa nepristupačnošću potraje najmanje 2-3 minuta

**Još uvek imam problema sa lozinkom sinhronizacijom**

- Ako i dalje imate poteškoća, pokušajte da onemogućite i ponovo omogućite uslugu "ispravnost lozinke" u alatki Azure AD Connect
- Da biste saznali više, pogledajte kako da [onemogućite i ponovo omogućite poništavanje lozinki.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
