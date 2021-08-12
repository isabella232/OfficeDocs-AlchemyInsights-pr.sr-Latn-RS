---
title: 451 4.7.0 Privremena greška servera. Pokušajte ponovo kasnije. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812589"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Privremena greška servera. Pokušajte ponovo kasnije. PRX4

Može se suočiti sa problemom prilikom slanja e-pošte preko funkcije Smarthost "smtp.office365.com" pomoću metoda prosleđivanja SMTP klijenta i dobijate grešku: "451 4.7.0 greška privremenog servera. Pokušajte ponovo kasnije. PRX4 je uglavnom privremeno". 

Uverite se da ne koristite deljeno poštansko sanduče za prosleđivanje SMTP klijenta jer metod prosleđivanja SMTP klijenta zahteva licencirano poštansko sanduče za slanje pošte. Međutim, ako ne koristite deljeno poštansko sanduče i problem i dalje postoji, proverite sledeće:

1. Omogućite SMTP prosleđivanje klijenta za licencirano poštansko sanduče koje se koristi pokretanjem ove PowerShell komande:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    ILI

    1. Idite na Microsoft 365 centar administracije > **aktivni korisnici** i izaberite korisnika.
    1. Idite na karticu Pošta > **Aplikacije za e-poštu >** **Upravljanje aplikacijama za e-poštu**. 
    1. Uverite se da **je potvrđena postavka Potvrda identiteta SMTP** (omogućeno).
    1. Izaberite **Sačuvaj promene**.
    
    Da biste omogućili SMTP potvrdu identiteta za celu organizaciju, pokrenite ovu komandu:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Napomi:** Iz bezbednosnih razloga, preporučuje se da omogućite SMTP potvrdu identiteta samo za poštansko sanduče koje se koristi. Postavka na nivou korisnika zamenje postavku nivoa organizacije.

2. Onemogućite Azure bezbednosne podrazumevane vrednosti tako što će na vrednost "Omogući **podrazumevane vrednosti bezbednosti" biti** **"Ne":**

    1. Prijavite se na Azure portal kao administrator za bezbednost, administrator uslovnog pristupa ili globalni administrator.
    1. Potražite svojstva Azure Active Directory >**  stavku**, a zatim izaberite **Upravljanje podrazumevanim vrednostima bezbednosti**.
    1. Postavite **preklopnik Omogući podrazumevane** vrednosti bezbednosti na **Ne**.
    1. Izaberite **Sačuvaj**.

3. Onemogućite uslugu Multi Factor Authentication (MFA) na licenciranom poštanskom sandučetu koje se koristi.

    1. Idite na prozor Microsoft 365 centar administracije u meniju navigacije sa leve strane odaberite stavku **Korisnici**  >  **aktivni korisnici.**
    1. Na stranici **Aktivni korisnici** odaberite stavku **Višestruka potvrda identiteta.**
    1. Izaberite korisnika i **onemogućite Multi-Factor Authentication**.

