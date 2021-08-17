---
title: Rešavanje problema sa nesumnjivim jedinstvenim prijavljivanjem (SSO) zasnovanim na OIDC-u
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
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105792"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Rešavanje problema sa nesumnjivim jedinstvenim prijavljivanjem (SSO) zasnovanim na OIDC-u

- Da biste saznali kako da dodate aplikaciju zasnovanu na OIDC-u u Azure zakupca, pogledajte brzi start: Podešavanje jedinstvenog prijavljivanje zasnovanog na [OIDC-u (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)za aplikaciju u Azure Active Directory (Azure AD) zakupcu.
- Više detalja o aplikacijama koje koriste OpenID Povezivanje za primenu jedinstvenog prijavljivanje, pogledajte razumevanje jedinstvenog prijavljivanje zasnovanog na [OIDC-u.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Informacije u slučaju da odaberete da napišete kôd tako što ćete direktno poslati HTTP zahteve i rukovanje tim zahtevima ili koristiti biblioteku otvorenog izvora nezavisnog dobavljača umesto korišćenja neke od biblioteka otvorenog izvora, pogledajte [OAuth 2.0 i OpenID Povezivanje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)protokole na Microsoft platforma za identitete.

**Protokoli**

1. [Microsoft platforma za identitete implicitnog](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) toka dodele – Definisanje karakteristike implicitne odobravanja je da se tokeni (ID tokeni ili tokeni za pristup) vraćaju direktno iz krajnje tačke /authorize umesto krajnje tačke /tokena. Ovo se često koristi kao deo toka koda autorizacije, koji se naziva **"hibridni tok" –** oduzivanje ID tokena u zahtevu za autorizacija zajedno sa kodom za autorizovanje. U ovom članku je opisano kako da direktno iz aplikacije program protiv protokola zatražite tokene od Azure AD.
2. Microsoft platforma za identitete i [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) tok koda za autorizovanje – OAuth 2.0 odobrenje koda za autorizovanje može da se koristi u aplikacijama koje su instalirane na uređaju za dobijanje pristupa zaštićenim resursima, kao što su veb A API-je. Pomoću primene Microsoft platforma za identitete OAuth 2.0, možete da dodate prijavljivanje i API pristup aplikacijama za mobilne uređaje i stone **računare.** U ovom članku se opisuje kako da se program prikazujete direktno u odnosu na protokol u aplikaciji na bilo kom jeziku.
3. [Microsoft platforma za identitete i OpenID Povezivanje](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) protokolu – Kada koristite primenu openID Povezivanje programa Microsoft platforma za identitete Povezivanje, možete da dodate prijavljivanje i pristup API-u aplikacijama. Ovaj članak vam pokazuje kako da to uradite nezavisno od jezika i opisuje kako da šaljete i primate HTTP poruke bez korišćenja **Microsoft biblioteke otvorenog izvora.**
4. Microsoft platforma za identitete klijenta i [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) tok akreditiva klijenta – OAuth 2.0 dodelu akreditiva klijenta navedenu u RFC 6749, koji se ponekad naziva **oAuth** sa dva leva, možete da koristite za pristup resursima hostovanim na vebu pomoću identiteta aplikacije. Ovaj tip odobravanja se obično koristi za interakcije između servera i servera koje moraju da se pokrenu u pozadini, bez neposredne interakcije sa korisnikom. Ovi tipovi aplikacija se često nazivaju **nalozima ili** nalozima **usluge.** Ovaj članak opisuje kako da se program prikazujete direktno u odnosu na protokol u vašoj aplikaciji.
