---
title: Problemi sa sistemom MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755145"
---
# <a name="issues-with-azure-mfa"></a>Problemi sa uslugom Azure MFA
Postoji nekoliko stvari koje treba da potvrdite ako korisnici ne mogu da se prijave pomoću multifaktor potvrde identiteta (MFA)

1. Pogođeni korisnik može biti blokiran na portalu Azure Active Directory. Ako je to slučaj, pokušaji potvrde identiteta za taj određeni korisnik se automatski odbijaju. [Pratite korake iz ovog članka da biste ih deblokirali.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ako deblokiranje korisnika nije pomogao ili korisnik nije blokiran, možete pokušati da poništite MFA za korisnika i oni će ponovo proći kroz proces unosa. [Pratite korake u ovom članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ako je ovo prvi put da omogućite MFA i vaši korisnici ne mogu da se prijave na klijente koji nisu u pregledaču, kao što su Outlook, Skype itd, možda ADAL (biblioteka potvrde identiteta Active Directory) nije omogućena na O365 pretplati. U ovom slučaju moraćete da se povežete sa uslugom Exchange online PowerShell i uradite ovaj cmdlet:  *setu-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*