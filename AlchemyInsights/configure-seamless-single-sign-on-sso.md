---
title: Konfigurisanje nesometanog jedinstvenog prijavljivanje (SSO)
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
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402281"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurisanje nesometanog jedinstvenog prijavljivanje (SSO)

**Konfigurisanje aplikacija**

1. Trebalo bi da dobijete vrednosti od prodavca aplikacije. Možete ručno da unesete vrednosti ili otpremite datoteku metapodataka da biste izdvojiti vrednost polja.
2. Mnoge aplikacije su već unapred konfigurisane za rad sa uslugom Azure AD. Ove aplikacije su navedene u galeriji aplikacija koje možete da pregledate kada dodate aplikaciju U Azure AD zakupca. Grupa [brzih startova](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) će vas proći kroz proces.
3. Da biste kreirali aplikaciju koja nije galerija, možete da kliknete na **dugme +** Kreirajte sopstvenu aplikaciju i date ime aplikaciji.
    - Podrazumevano će izabrati opciju Integriši sve druge aplikacije koje ne pronađete u galeriji, što je ispravna opcija za **aplikacije** koje nisu u galeriji.
    - Kada **pritisnete** stavku Kreiraj nakon što stavite ime za aplikaciju, kreiraće se nova enterprise aplikacija koja nije galerija.
    - Zatim možete da odete  na jedinstveno  prijavljivanje u okviru Upravljanje tom aplikacijom i moći ćete da vidite različite tehnike za primenu u okruženju.

**Konfigurisanje nesomećenog SSO-a za određenu aplikaciju**

Za aplikacije u galeriji ćete pronaći detaljna uputstva korak po korak. Da biste pristupili koracima, možete da pregledate listu svih uučavanja za konfiguraciju aplikacije u uputstvima za konfiguraciju [SaaS aplikacije.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfigurisanje SSO zasnovanog na SAML-u**

1. Brzi start: Podešavanje jedinstvenog prijavljivanje zasnovanog na [SAML-u (SSO) za aplikaciju u Azure Active Directory (Azure AD) zakupca.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Da biste saznali više o opciji zasnovanoj na SAML-u za jedinstveno prijavljivanje, pogledajte razumevanje jedinstvenog prijavljivanje zasnovanog na [SAML-u.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Da biste saznali više o ZAHTEVima za SAML 2.0 potvrdom identiteta i odgovorima koje Azure Active Directory (Azure AD) podržava za Single Sign-On (SSO), pogledajte [single Sign-On SAML protokol.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Da biste saznali kako da kreirate i konfigurišete jedinstveno prijavljivanje zasnovano na SAML-u (SSO) za aplikaciju u sistemu Azure Active Directory (Azure AD) koristeći Microsoft Graph API, pogledajte članak Konfigurisanje jedinstvenog prijavljivanje zasnovanog na [SAML-u](https://docs.microsoft.com/graph/application-saml-sso-configure-api)za aplikaciju pomoću microsoft Graph API-ja.
5. Da biste saznali kako Azure AD koristi SAML protokol, pogledajte članak [Kako platforma Microsoft identitet koristi SAML protokol.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfigurisanje tokena i zahteva**

1. [Kako da: prilagodite zahteve izdate u SAML tokenu za poslovne aplikacije.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Da biste saznali kako da konfigurišete zahteve pomoću programa PowerShell, pogledajte kako da: prilagodite zahteve emitovane u tokenima za određenu aplikaciju u zakupca [(Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Da biste saznali kako da konfigurišete opcionalne zahteve, pogledajte kako da: pružite [opcionalne zahteve aplikaciji.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Da biste saznali kako da koristite atribute proširenja šeme direktorijuma za slanje korisničkih podataka aplikacijama u zahtevima za token, pogledajte temu Korišćenje atributa proširenja [šeme direktorijuma u zahtevima.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Da biste saznali kako da konfigurišete trajanja tokena, pogledajte članak Konfigurisanje trajanja [tokena na platformi Microsoft identitet (pregled).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfigurisanje smernica za](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) trajanje tokena (pregled) – U ovom članku ćemo proći kroz scenario uobičajenih smernica koji vam može pomoći da nametnete nova pravila za trajanje tokena. U primeru ćete saznati kako da kreirate smernice koje zahtevaju da korisnici češće potvrde identitet u veb aplikaciji.

**Rešavanje problema sa SSO konfiguracijom**

- Za najčešća pitanja o Azure Active Directory nesumnjivom jedinstvenom Sign-On (nesmanje SSO), pogledajte [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)nesmanje jedinstveno prijavljivanje: najčešća pitanja.
- Za informacije o rešavanju uobičajenih problema u vezi sa nesmašnim jedinstvenim prijavljivanjem za Azure Active Directory (Azure A Sign-On D), pogledajte rešavanje problema sa nesumnjivim jedinstvenim prijavljivanjem u [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
