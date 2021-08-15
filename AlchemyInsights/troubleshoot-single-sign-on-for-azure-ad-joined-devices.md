---
title: Rešavanje problema sa jedinstvenim prijavljivanjem za Azure AD pridružene uređaje
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
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039260"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Rešavanje problema sa jedinstvenim prijavljivanjem za Azure AD pridružene uređaje

Ako imate okruženje iz usluge Active Directory (AD) i želite da se pridružite računarima pridruženim AD domenu u uslugu Azure AD, to možete da postignete tako što ćete izvršiti hibridno Azure AD pridruživanje. [Kako da: planirate hibridnu primenu Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) spajanja pružaju vam srodne korake za primenu hibridnog Azure AD pridruživanja u okruženju.

Dodatne informacije potražite u Single-Sign Konfigurisanje [Azure AD](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)pridruženih uređaja za Single-Sign On using Windows Hello for Business .

**Problemi sa primarnim tokenim osvežavanja (PRT)**

Primarni token za osvežavanje (PRT) je ključni artifakt Azure AD potvrde identiteta na Windows 10, Windows Server 2016 i novijim verzijama, iOS i Android uređajima. To je JSON veb token (JWT) posebno izdat Microsoft raskidačima tokena za prve strane kako bi se omogućilo jedinstveno prijavljivanje (SSO) u svim aplikacijama koje se koriste na tim uređajima. Detalje o tome kako se PRT izdaje, koristi i štiti na Windows 10 uređajima, pogledajte šta je to primarni [token za osvežavanje?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: YES i AzureADPrt: YES**

Ova polja ukazuju na to da li je korisnik uspešno potvrdio identitet za Azure AD prilikom prijave na uređaj. Ako su vrednosti **NE,** to može biti zbog:

- Loš ključ za skladištenje u TPM-u povezanom sa uređajem nakon registracije (proverite KeySignTest dok je pokrenut sa punim punim brojem)
- Alternativni ID za prijavljivanje
- HTTP proxy nije pronađen

Da biste rešili probleme sa uređajima pomoću dsregcmd komande, pogledajte [SSO stanje.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
