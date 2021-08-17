---
title: Rešavanje problema sa SSPR-om
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038972"
---
# <a name="troubleshoot-sspr"></a>Rešavanje problema sa SSPR-om

**Imam problema pri konfigurisanju poništavanja lozinke**

- Ako ste administrator i tražite kako da omogućite samouslužno poništavanje lozinke, pogledajte uputstvo za [omogućavanje usluge SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)za konfigurisanje poništavanje lozinke za organizaciju. Možda ćete želeti i da [pregledate zahteve za licenciranje.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) Morate imati barem jednu licencu dodeljenu u organizaciji.
    - **Samo korisnici u oblaku** – Svi Office 365 (O365) plaćeni SKU ili Azure AD Basic
    - **Oblak i/ili** korisnici – Azure AD Premium P1 ili P2, Enterprise Mobility + Security (EMS) ili Secure Productive Enterprise (SPE)
- Za dodatna pitanja o samouslužnom poništavanje lozinke, pregledajte [najčešća pitanja.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**Dobijam poruku o grešci**

Pregledajte ovaj članak da biste pronašli uobičajene greške i njihova rešenja: Rešavanje problema sa [samouslužnim poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Imam problem sa smernicama za poništavanje lozinke**

- Ako se smernice za poništavanje lozinke ne ponašaju na očekivani način ili ako imate pitanja o smernicama za poništavanje lozinke, pregledajte ovaj članak: Smernice i ograničenja lozinke u [okviru Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- Smernice za poništavanje lozinke ne primenjuju se na administratore. Microsoft nalaže jake smernice za poništavanje lozinke sa dva mrežna prolaza za svaku ulogu administratora usluge Azure. Proverite da li testirate sa korisnikom koji nije administrator. Više informacija o smernicama za poništavanje administratora potražite u ovom članku: [Razlike u smernicama administratora za poništavanje.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**Ne želim da korisnici registruju dodatne bezbednosne informacije za poništavanje lozinke**

Možete unapred da popunite podatke (atribute e-pošte i telefona) za korisnike pomoću API-ja, programa PowerShell ili Azure AD Povezivanje. Da biste saznali kako da čitate:

- [Primena poništavanja lozinke bez korisnika koji moraju da se registruju](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Koje podatke poništavanje lozinke koristi](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Želim da moji korisnici registruju dodatne bezbednosne informacije za poništavanje lozinke**

1. Neka korisnici registruju svoje bezbednosne informacije za samouslužno poništavanje lozinke tako što će ih usmeriti [na aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)
1. Kada se podaci za korisnika (odrede korisnik ili od strane korisnika), usmerite korisnika da koristi [aka.ms/sspr](https://passwordreset.microsoftonline.com/) kako bi korisnici mogli da se podstaknu da ponište sopstvene lozinke.
1. Ako korisnici i dalje nailazite na probleme ako su najverovatnije **fedeterni korisnici** ili korisnici koji **imaju sinhronizovanu** lozinku. To znači da verovatno postoji problem sa uslugom "Pisanje lozinke".