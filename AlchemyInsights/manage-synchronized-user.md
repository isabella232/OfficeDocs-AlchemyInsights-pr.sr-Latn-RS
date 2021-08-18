---
title: Upravljanje sinhronizovanim korisnikom
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114792"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nije moguće podesiti primarnu adresu e-pošte, promeniti atribute korisnika ili ukloniti/izbrisati sinhronizovanog korisnika

Ako je sinhronizacija direktorijuma omogućena za okruženje, pojedini atributi korisnika ili objekta ne mogu da se promene pomoću Microsoft 365 centar administracije.

Da biste u potpunosti upravljali sinhronizovanim korisnicima i svim njihovim atributima, koristite lokalne active directory korisnike i konzolu za upravljanje grupama (adsiedit.msc).  

Druga mogućnost je da promenite pojedinačne korisnike ili atribute za sinhronizovane korisnike pomoću programa powershell, kao što je prikazano u ovim uobičajenim primerima:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
