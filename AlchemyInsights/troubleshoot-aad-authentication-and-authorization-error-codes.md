---
title: Rešavanje problema sa kodom Azure AD potvrde identiteta i autorizacije (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037837"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Rešavanje problema sa kodom Azure AD potvrde identiteta i autorizacije (AADSTS)

Da biste rešili AAD potvrde identiteta i lozinke (AADSTS), obavite sledeće preporučene korake:

1. **Rukovanje šifri grešaka u aplikaciji**

- **OAuth 2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2 pruža uputstva za rukovanje greškama tokom potvrde identiteta pomoću dela greške na osnovu odgovora na grešku.

    - **Greška**: niska koda greške koja se može koristiti za klasifikaciju tipova grešaka koje se javljaju i treba da se koristi za reagovanje na greške.
    - Polje " **Greška** " ima nekoliko mogućih vrednosti – pregledajte veze podataka protokola i OAuth 2,0 specifikacije za više informacija o određenim greškama i kako da reagujete na njih.

- Evo uzorka odgovora o grešci:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Pronalaženje trenutnih informacija sa kodom greške**

- Kodovi grešaka i poruke podležu promenama. Za najnovije informacije pogledajte https://login.microsoftonline.com/error stranicu da biste pronašli AADSTS opise grešaka, ispravke i neka predložena rešenja.
- Možete da tražite i rešite probleme sa [kodom greške](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) koji su navedeni u članku [Azure AD potvrda identiteta i lozinke](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Nabavite pomoć**

- [Opcije podrške i pomoći za programere](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – ako vam je potreban odgovor na pitanje ili pomoć u rešavanju problema koji nije obuhvaćena naљom dokumentacijom, možda je vreme da se obratite ekspertima za pomoć. Ovaj članak pruža nekoliko predloga za dobijanje odgovora na pitanja dok razvijate aplikacije koje se integrišu sa Microsoft platformom identiteta.








