---
title: Problemi sa Simbomnim tvrdnjama i atributima
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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035971"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemi sa Simbomnim tvrdnjama i atributima

**Ažuriranje, konfigurisanje ili uklanjanje simbola simbola**

1. Pomoću Azure aktivnog direktorijuma (Azure AD) možete da [prilagodite tip zahteva za pretenzije](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) na oznaku za odgovor koji primite kada odobrite aplikaciju.
2. Programeri aplikacije mogu da koriste opcionalne zahteve u svojim Azure AD aplikacijama da bi naveli koje tvrdnje žele u željama koje su poslate u aplikaciju. Više informacija potražite u članku [obezbeđivanje opcionalnih tvrdnji za aplikaciju](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Podesite grupne zahteve za aplikacije pomoću usluge Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Ako koristite Nesmetna jedinstveno prijavljivanje u aplikaciji, pogledajte članak [Prilagođavanje tvrdnji izdatih u znaku semla za preduzeća](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Mapiranje atributa potraživanja**

1. Da biste konfigurisali smernice za mapiranje potraživanja pomoću programa PowerShell, pogledajte članak [Prilagođavanje tvrdnji koje se automatski emituje za određenu aplikaciju u zakupcu (pregled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Atributi proširenja šeme direktorijuma obezbeđuju način skladištenja dodatnih podataka u usluzi Azure Active Directory na korisničkim objektima i drugim objektima direktorijuma kao što su grupe, detalji zakupca, direktori usluga. Samo produženi atributi na korisničkim objektima mogu da se koriste za emitovanje tvrdnji u aplikacijama. [Korišćenje atributa proširenja šeme direktorijuma u tvrdnjama](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) objašnjava kako se koriste atributi proširenja šeme direktorijuma za slanje korisničkih podataka u aplikacije u zahtevima za Token.

Više informacija o simbomnoj tvrdnji potražite u članku:

- [Potraživanja u Access tokenima](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Zahtevi u id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Tvrdnje](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) koje možete OČEKIVATI od ID-ova i Access tokena koje izda AZURE AD B2C
- [Zahtev za SEML Token](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
