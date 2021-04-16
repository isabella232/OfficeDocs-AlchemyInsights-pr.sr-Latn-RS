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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="4bae0-102">Problemi sa Azure MFA</span><span class="sxs-lookup"><span data-stu-id="4bae0-102">Issues with Azure MFA</span></span>
<span data-ttu-id="4bae0-103">Postoji nekoliko stvari koje treba da proverite ako korisnici ne mogu da se prijade pomoću višestruke potvrde identiteta (MFA)</span><span class="sxs-lookup"><span data-stu-id="4bae0-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="4bae0-104">Korisnik na koji ovo utiče može biti blokiran na Azure Active Directory portalu.</span><span class="sxs-lookup"><span data-stu-id="4bae0-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="4bae0-105">Ako je to slučaj, pokušaji potvrde identiteta za tog određenog korisnika biće automatski odbijeni.</span><span class="sxs-lookup"><span data-stu-id="4bae0-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="4bae0-106">Pratite korake u ovom članku da biste ih deblokirali.</span><span class="sxs-lookup"><span data-stu-id="4bae0-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="4bae0-107">Ako deblokiranje korisnika nije pomoglo ili nije blokirano, možete pokušati da uspostavite početne vrednosti usluge MFA za korisnika i on će ponovo proći kroz proces uređivanja.</span><span class="sxs-lookup"><span data-stu-id="4bae0-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="4bae0-108">Pratite korake iz ovog članka.</span><span class="sxs-lookup"><span data-stu-id="4bae0-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="4bae0-109">Ako prvi put omogućite MFA i korisnici ne mogu da se prijave u klijente koji nisu pregledači kao što su Outlook, Skype itd, možda UDAL (Active Directory biblioteka potvrde identiteta) nije omogućena u O365 pretplati.</span><span class="sxs-lookup"><span data-stu-id="4bae0-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="4bae0-110">U ovom slučaju ćete morati da se povežete sa uslugom Exchange Online Powershell i pokrenete ovu cmdlet  *datoteku: Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="4bae0-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>