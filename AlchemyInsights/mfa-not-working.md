---
title: Problemi sa MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098616"
---
# <a name="issues-with-azure-mfa"></a>Problemi sa Azure MFA
Postoji nekoliko stvari koje treba da proverite ako korisnici ne mogu da se prijade pomoću višestruke potvrde identiteta (MFA)

1. Korisnik na koji ovo utiče može biti blokiran na Azure Active Directory Portalu. Ako je to slučaj, pokušaji potvrde identiteta za tog određenog korisnika biće automatski odbijeni. [Pratite korake u ovom članku da biste ih deblokirali.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ako deblokiranje korisnika nije pomoglo ili nije blokirano, možete pokušati da uspostavite početne vrednosti usluge MFA za korisnika i on će ponovo proći kroz proces uređivanja. [Pratite korake iz ovog članka.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ako prvi put omogućite MFA i korisnici ne mogu da se prijave na klijente koji nisu pregledači, kao što su Outlook, Skype itd, možda ADAL (Active Directory biblioteka potvrde identiteta) nije omogućena u O365 pretplati. U ovom slučaju ćete morati da se povežete sa Exchange Online Powershell i pokrenete ovu cmdlet *datoteku: Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*