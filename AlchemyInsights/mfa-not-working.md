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
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810498"
---
# <a name="issues-with-azure-mfa"></a>Problemi sa Azure MFA
Postoji nekoliko stvari koje treba da proverite ako korisnici ne mogu da se prijade pomoću višestruke potvrde identiteta (MFA)

1. Korisnik na koji ovo utiče može biti blokiran na Azure Active Directory portalu. Ako je to slučaj, pokušaji potvrde identiteta za tog određenog korisnika biće automatski odbijeni. [Pratite korake u ovom članku da biste ih deblokirali.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ako deblokiranje korisnika nije pomoglo ili nije blokirano, možete pokušati da uspostavite početne vrednosti usluge MFA za korisnika i on će ponovo proći kroz proces uređivanja. [Pratite korake iz ovog članka.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ako prvi put omogućite MFA i korisnici ne mogu da se prijave u klijente koji nisu pregledači kao što su Outlook, Skype itd, možda UDAL (Active Directory biblioteka potvrde identiteta) nije omogućena u O365 pretplati. U ovom slučaju ćete morati da se povežete sa uslugom Exchange Online Powershell i pokrenete ovu cmdlet  *datoteku: Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*