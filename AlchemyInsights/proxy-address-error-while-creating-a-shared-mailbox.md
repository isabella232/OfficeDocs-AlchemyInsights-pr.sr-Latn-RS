---
title: Greška proxy adrese prilikom kreiranja deljenog poštanskog sandučeta
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568304"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Greška proxy adrese prilikom kreiranja poštanskog sandučeta ili drugog objekta omogućenog e-pošte

Ako ste pokušali da kreirate objekat sa omogućenom e-poštom (poštansko sanduče, Deljeno poštansko sanduče itd.) i dobili grešku "Proxy adresa" SMTP:alias@domain.com "se već koristi...", e-adresa koju ste odabrali već je uzeta drugi objekat sa omogućenim e-adresom u organizaciji.
  
Potrebno je da pronađete korisnika, grupu, Deljeno poštansko sanduče ili javnu fasciklu koja ima ovu e-adresu i da je izbriše ili da promeni adresu e-pošte. Zatim možete da kreirate novi objekat sa omogućenom e-poštom sa oslobođenom adresom e-pošte. Koristite pretragu na matičnoj stranici da biste je pronašli. Možete da koristite i sledeću Exchange online komandu PowerShell da biste je pretražili:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ako ne želite da izbrišete postojeću adresu e-pošte, odaberite novu e-adresu za novi objekat koji kreirate.
  