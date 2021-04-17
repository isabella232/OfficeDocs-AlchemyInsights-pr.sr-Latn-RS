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
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823981"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nije moguće podesiti primarnu adresu e-pošte, promeniti atribute korisnika ili ukloniti/izbrisati sinhronizovanog korisnika

Ako je sinhronizacija direktorijuma omogućena za okruženje, neki atributi korisnika ili objekta ne mogu da se promene pomoću Microsoft 365 centra za atribute.

Da biste u potpunosti upravljali sinhronizovanim korisnicima i svim njihovim atributima, koristite lokalne active directory korisnike i konzolu za upravljanje grupama (adsiedit.msc).  

Druga mogućnost je da promenite pojedinačne korisnike ili atribute za sinhronizovane korisnike pomoću programa powershell, kao što je prikazano u ovim uobičajenim primerima:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
