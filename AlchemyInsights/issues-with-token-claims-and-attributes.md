---
title: Problemi sa zahtevima i atributima tokena
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012898"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemi sa zahtevima i atributima tokena

**Ažuriranje, konfigurisanje ili uklanjanje zahteva tokena**

1. Korišćenjem Azure Active Directory (Azure AD), možete [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) da prilagodite tip zahteva za zahtev uloge u tokenu odgovora koji primite kada ovlastite aplikaciju.
2. Projektanti aplikacije mogu da koriste opcionalne zahteve u Azure AD aplikacijama da bi naveli koje zahteve žele u tokenima koji se šalju aplikaciji. Dodatne informacije potražite u [temi Naveli opcionalne zahteve za aplikaciju.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurišite grupne zahteve za aplikacije Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ako koristite nesometno jedinstveno prijavljivanje u aplikaciji, pogledajte prilagođavanje zahteva izdatih u [SAML tokenu za poslovne aplikacije.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Mapiranje atributa "Zahtevi"**

1. Da biste konfigurisali smernice za mapiranje zahteva pomoću programa PowerShell, pogledajte prilagodite zahteve emitovane u tokenima za određenu aplikaciju u zakupca [(Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Atributi proširenja šeme direktorijuma pružaju način za skladištenje dodatnih podataka u Azure Active Directory na objektima korisnika i drugim objektima direktorijuma kao što su grupe, detalji o zakupcu, principali usluga. Samo atributi proširenja u objektima korisnika mogu da se koriste za emitiranje tužbi u aplikacijama. Korišćenje atributa proširenja šeme direktorijuma u zahtevima opisuje kako da [koristite](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) atribute proširenja šeme direktorijuma za slanje korisničkih podataka aplikacijama u tužbama tokena.

Više informacija o zahtevima za token potražite u:

- [Zahtevi u tokenima za pristup](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Zahtevi u id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Zahtevi koje](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) možete da očekujete u ID tokenima i tokenima za pristup koje izdaje Azure AD B2C
- [Referenca za zahteve za SAML token](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
