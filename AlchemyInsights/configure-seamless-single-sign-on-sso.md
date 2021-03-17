---
title: Konfigurisanje besprekornog jedinstvenog prijavljivanja (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841674"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurisanje besprekornog jedinstvenog prijavljivanja (SSO)

**Konfigurisanje aplikacija**

1. Trebalo bi da nabavite vrednosti od dobavljača aplikacije. Možete ručno da unesete vrednosti ili da otpremite datoteku metapodataka da biste izdvojili vrednost polja.
2. Mnoge aplikacije su već unapred konfigurisane za rad sa uslugom Azure AD. Ove aplikacije su navedene u galeriji aplikacija koje možete da pregledate kada dodate aplikaciju u Azure AD stanar. [Brza grupa](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vas prolazi kroz proces.
3. Da biste kreirali aplikaciju koja nije galerija, možete da kliknete na dugme Uključi **+ Kreiranje sopstvene aplikacije** i date ime aplikaciji.
    - Podrazumevano, ona će izabrati stavku **integrisati bilo koju drugu aplikaciju koju ne pronađete u galeriji** koja je ispravna opcija za aplikacije koje nisu iz galerije.
    - Kada **unesete ime** za aplikaciju, on će kreirati novu aplikaciju preduzeća koja nije galerija.
    - Zatim možete da se krećete na **jedinstveno prijavljivanje** u okviru **upravljanja** tom aplikacijom i moći ćete da vidite različitu tehniku za primenu u okruženju.

**Konfigurisanje besprekornog SSO za određenu aplikaciju**

Za aplikacije u galeriji videćete detaljnu, postepenog, uputstva. Da biste pristupili koracima, možete da pregledate listu svih uputstava za konfiguraciju aplikacije na [uputstvima za konfiguraciju aplikacije Sahas](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Konfigurišite SSO sa sistemom SEML**

1. [Brzi Start: podesite SAML-ova Single za prijavljivanje (SSO) za aplikaciju u Azure Active Directory (AZURE AD) zakupcu](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Da biste saznali više o opciji zasnovano na jedinstvenom prijavljivanje, pogledajte članak [razumevanje jednostrukog prijavljivanja na osnovu Sema l](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Da biste saznali više o zahtjevima za potvrdu identiteta za SAML 2,0 i odgovore da Azure Active Directory (Azure AD) podržava jednokratnu Sign-On (SSO), pogledajte članak [Single Sign-On seml protokol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Da biste saznali kako da kreirate i konfigurišete Single-in za jedinstveno prijavljivanje (SSO) za aplikaciju u usluzi Azure Active Directory (Azure AD) pomoću Microsoft Graph API, pogledajte članak [Konfigurisanje SAML-a jedinstvenog prijavljivanja za aplikaciju pomoću Microsoft Graph API](https://docs.microsoft.com/graph/application-saml-sso-configure-api)-ja.
5. Da biste saznali kako Azure AD koristi SAML protokol, pogledajte [kako Microsoft funkcija za identifikaciju koristi saml protokol](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfigurisanje Tikena i tvrdnji**

1. [Kako da: prilagodite tvrdnje izdate iz znaka seml za preduzeća](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Da biste saznali kako da konfigurišete zahteve pomoću programa PowerShell, pogledajte članak [: prilagođavanje tvrdnji koji se automatski emituje za određenu aplikaciju u zakupcu (pregled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Da biste saznali kako da konfigurišete opcionalne tužbe, pogledajte članak [: obezbeđivanje opcionalnih tvrdnji za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Da biste saznali kako da koristite atribute proširenja šeme direktorijuma za slanje korisničkih podataka u aplikacije u zahtevima za oznaku simbola, pogledajte članak [Korišćenje atributa proširenja šeme direktorijuma u zahtevima](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Da biste saznali kako da konfigurišete Token ћivota, pogledajte članak [Pregled simbola koji je moguće konfigurisati u Microsoft platformi identiteta (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfigurisanje simbola trajanja tokena (Preview)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) -u ovom članku prošećemo kroz uobičajen scenarij koji može da vam pomogne da nametnete nova pravila za životni vek. U primeru, naučite kako da kreirate smernice koje zahtevaju da korisnici češće rade autentičnosti u Veb aplikaciji.

**Rešavanje problema sa konfiguracijom SSO**

- Najčešća pitanja o Azure Active Directory Nesmetna Sign-On (besprekoran SSO) potražite u članku [Azure Active Directory nije pristupačnija jednostruko prijavljivanje: najčešća pitanja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Za rešavanje problema sa informacijama o uobičajenim problemima koji se tiču Azure aktivnog direktorijuma (Azure AD) bez slobodne Sign-On (besprekorni SSO) pogledajte članak [Rešavanje problema sa uslugom Azure Active Directory nije jedinstveno prijavljivanje](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
