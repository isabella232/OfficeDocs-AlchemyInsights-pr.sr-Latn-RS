---
title: Single-Sign je za pridružene Azure Active Directory uređaje
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050024"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Jedinstveno prijavljivanje za uređaje Azure Active Directory pridružene uređaje

Ako imate okruženje iz usluge Active Directory (AD) i želite da se pridružite računarima pridruženim AD domenu u uslugu Azure AD, to možete da postignete tako što ćete izvršiti hibridno Azure AD pridruživanje. [Kako da: planirate hibridnu primenu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) spajanja pružaju vam srodne korake za primenu hibridnog Azure AD pridruživanja u okruženju.

[Konfigurisanje Azure AD pridruženih uređaja za Single-Sign Na korišćenje usluge Windows Hello za preduzeća](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemi sa primarnim tokenim osvežavanja (PRT)** Primarni token za osvežavanje (PRT) je ključni artifakt Azure AD potvrde identiteta na Windows 10, Windows Server 2016 i novijim verzijama, iOS i Android uređajima. To je JSON veb token (JWT) posebno izdat Microsoft raskidačima tokena za prve strane kako bi se omogućilo jedinstveno prijavljivanje (SSO) u svim aplikacijama koje se koriste na tim uređajima. [U 1.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)izdanju Šta je to primarni token za osvežavanje? pružićemo detalje o tome kako se PRT izdaje, koristi i štiti na Windows 10 uređajima.

**WamDefaultSet: YES i AzureADPrt: YES** Ova polja ukazuju na to da li je korisnik uspešno potvrdio identitet za Azure AD prilikom prijave na uređaj. Ako su vrednosti **NE**, može biti krajnji rok:

- Loš ključ za skladištenje u TPM-u povezanom sa uređajem nakon registracije (proverite KeySignTest dok ste pokrenuti sa punim punim brojem).
- Alternativni ID za prijavljivanje
- HTTP proxy nije pronađen

Rešavanje problema sa uređajima pomoću dsregcmd komande – [SSO stanje](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
