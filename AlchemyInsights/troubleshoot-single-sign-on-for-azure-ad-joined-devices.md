---
title: Rešavanje problema sa jednim znakom za Azure AD koji se pridružuje
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
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037331"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Rešavanje problema sa jednim znakom za Azure AD koji se pridružuje

Ako imate lokalno okruženje aktivnog direktorijuma (AD) i želite da se pridružite OGLAŠAVANJU računara koji su se pridružili programu Azure AD, to možete da postignete tako što ćete postupiti na hibridnu Azure AD. [Kako da: planirate hibridno Azure Active Directory pridruživanje](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vam pruža srodne korake za primenu hibridnog AZURE oglašavanja u okruženju.

Više informacija potražite u članku [Konfigurisanje Azure AD za priključene uređaje za lokalno Single-Sign na korišćenje Windows Helo za preduzeća](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Problemi sa Token osvežavanja (PRT)**

Primarni Token osvežavanja (PRT) je ključni artefakt za Azure AD potvrda identiteta u operativnom sistemu Windows 10, Windows Server 2016 i novije verzije, iOS i Android uređajima. To je JSON Veb Token (JWT) naročito izdat Microsoft brokerima za potpisivanje simbola, kako bi omogućili jedinstveno prijavljivanje (SSO) u aplikacijama koje se koriste na tim uređajima. Detalje o tome kako se PRT izdaje, koristi i štiti na Windows 10 uređajima potražite u članku [Šta je to simbol primarnog osvežavanja?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**Vamdefaultsceno: da i AzureADPrt: da**

Ova polja ukazuju na to da li je korisnik uspešno potvrdio pristup Azure AD kada se prijavi na uređaj. Ako vrednosti **nisu, to** može da bude zbog:

- Neispravan ključ skladišta u TPM-u koji je povezan sa uređajem po registraciji (Potvrdite prijavljivanje prilikom pokretanja povećanog)
- Alternativni ID prijavljivanja
- HTTP proxy nije pronađen

Da biste rešili probleme sa uređajima pomoću komande dsregcmd, pogledajte članak [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
