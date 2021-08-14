---
title: Greška adrese proxy servera prilikom kreiranja deljenog poštanskog sandučeta
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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062922"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Greška proxy adrese prilikom kreiranja poštanskog sandučeta ili drugog objekta omogućenog za e-poštu

Ako ste pokušali da kreirate objekat sa omogućenom e-poštom (poštansko sanduče, deljeno poštansko sanduče itd.) i dobili grešku "Proxy adresa "SMTP:alias@domain.com" se već koristi...", adresu e-pošte koji ste odabrali je već uzeo drugi objekat omogućen za e-poštu u organizaciji.
  
Treba da pronađete korisnika, grupu, deljeno poštansko sanduče ili javnu fasciklu koja sadrži ovu adresu e-pošte i izbrišete je ili promenite njegovu adresu e-pošte. Zatim možete da napravite novi objekat omogućen za e-poštu sa besplatnom e-adresom. Koristite pretragu na matičnoj stranici da biste je pronašli. Možete da koristite i sledeću Exchange Online PowerShell da biste je potražili:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ako ne želite da izbrišete postojeću adresu e-pošte, odaberite novu adresu e-pošte za novi objekat koji kreirate.
  