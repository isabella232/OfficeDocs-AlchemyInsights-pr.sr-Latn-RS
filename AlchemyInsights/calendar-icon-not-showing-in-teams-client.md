---
title: Ikona kalendara se ne prikazuje u Teams klijentu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989605"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Ikona kalendara se ne prikazuje u Teams klijentu

Kartica „Kalendar“ u usluzi Teams zahteva pristup Exchange poštanskom sandučetu putem veb usluga programa Exchange. Exchange poštansko sanduče može da bude na mreži ili lokalno. Za korisnike na mreži koji ne vide karticu „Kalendar“, uverite se da su [licencirani za Exchange Online poštansko sanduče i da je poštansko sanduče omogućeno](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ako korisnik ima važeće poštansko sanduče u usluzi Exchange Online, ali i dalje ne može da vidi karticu „Kalendar“, možda imate problem sa mrežom. Koristite [Microsoft analizator daljinske mogućnosti povezivanja](https://testconnectivity.microsoft.com/) i pokrenite **Microsoft Exchange testove mogućnosti povezivanja veb usluga** za korisnika na koga ovo utiče.

Na kraju proverite [Teams aplikacije – smernice za podešavanje aplikacija](https://admin.teams.microsoft.com/policies/app-setup) da biste se uverili da aplikacija Kalendar nije uklonjena iz smernica primenjenih na korisnika (verovatno su u pitanju **Globalne (podrazumevane za celu organizaciju)**.

Ako vaši korisnici rade lokalno kod kuće, treba da potvrdite da je vaša hibridna konfiguracija ispravna. Koristite [Čarobnjak za hibridnu konfiguraciju](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) da biste rešili problem.

Imajte u vidu da [Teams zahteva Exchange 2016 CU3 ili noviju verziju](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
