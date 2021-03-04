---
title: Rešavanje problema sa SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430216"
---
# <a name="troubleshoot-sspr"></a>Rešavanje problema sa SSPR

**Imam problema sa konfigurisanjem poništavanja lozinke**

- Ako ste administrator i tražite kako da omogućite samouslužno poništavanje lozinke, pogledajte [članak uputstvo za omogućavanje SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)da biste konfigurisali poništavanje lozinke za organizaciju. Možda ćete želeti da pregledate i [zahteve za licenciranje](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). Morate da imate najmanje jednu licencu dodeljenu u organizaciji.
    - **Samo oblaci korisnici** – bilo koji Office 365 (O365) plaćeni MJ ili AZURE AD Basic
    - **Cloud i/ili lokalno korisnici** – AZURE AD Premium P1 ili P2, Enterprise mobilnost + Security (Ems) ili bezbedno preduzeće (SPE)
- Za dodatna pitanja o poništavanju lozinke za samouslužno, pregledajte [naša najčešća pitanja](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Dobijam poruku o grešci**

Pregledajte ovaj članak da biste pronašli uobičajene greške i njihova rešenja: [Rešavanje problema samouslužnog poništavanja lozinke](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Imam problem sa smernicama za poništavanje lozinke**

- Ako se vaša smernica za poništavanje lozinke ne ponaša po očekivanom ili ako imate pitanja o smernicama za poništavanje lozinki, pregledajte ovaj članak: [smernice za lozinke i ograničenja u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- Smernice za poništavanje lozinke se ne primenjuju na administratore. Korporacija Microsoft obavezuje podrazumevane smernice za poništavanje lozinke sa dva vrata za bilo koju ulogu usluge Azure. Uverite se da testirate sa korisnikom koji nije administrator. Više informacija o administratorskim smernicama administratora potražite u članku: administrator je [poništilo razlike u smernicama](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Ne želim da moji korisnici registruju dodatne bezbednosne informacije za poništavanje lozinke**

Možete unapred da popunjavate podatke (e-poštu i telefonske atribute) za korisnike koristeći API, PowerShell ili Azure AD Connect. Da biste saznali kako se čita:

- [Primena početne vrednosti poništavanja bez potrebe korisnika da se registruju](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Koje podatke koristi poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Želim da moji korisnici registruju dodatne bezbednosne informacije za poništavanje lozinke**

1. Neka vaši korisnici registruju svoje bezbednosne informacije za poništavanje lozinke samouslužavanja tako što ćete ih usmeriti na [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).
1. Kada su podaci naseljeni za korisnika (korisnik ili administrator), usmerite korisnika na [aka.MS/sspr](https://passwordreset.microsoftonline.com/) kako bi korisnici mogli da imaju ovlašćenja da ponovo postave sopstvene lozinke.
1. Ako korisnici i dalje imaju **problema, oni su najverovatnije automatski** automatski ili **hash sinhronizovanje lozinki** . To znači da je verovatno problem sa uslugom poništavanje lozinki.