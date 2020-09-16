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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="cced6-102">Problemi sa uslugom Azure MFA</span><span class="sxs-lookup"><span data-stu-id="cced6-102">Issues with Azure MFA</span></span>
<span data-ttu-id="cced6-103">Postoji nekoliko stvari koje treba da potvrdite ako korisnici ne mogu da se prijave pomoću multifaktor potvrde identiteta (MFA)</span><span class="sxs-lookup"><span data-stu-id="cced6-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cced6-104">Pogođeni korisnik može biti blokiran na portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cced6-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cced6-105">Ako je to slučaj, pokušaji potvrde identiteta za taj određeni korisnik se automatski odbijaju.</span><span class="sxs-lookup"><span data-stu-id="cced6-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cced6-106">Pratite korake iz ovog članka da biste ih deblokirali.</span><span class="sxs-lookup"><span data-stu-id="cced6-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cced6-107">Ako deblokiranje korisnika nije pomogao ili korisnik nije blokiran, možete pokušati da poništite MFA za korisnika i oni će ponovo proći kroz proces unosa.</span><span class="sxs-lookup"><span data-stu-id="cced6-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cced6-108">Pratite korake u ovom članku.</span><span class="sxs-lookup"><span data-stu-id="cced6-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cced6-109">Ako je ovo prvi put da omogućite MFA i vaši korisnici ne mogu da se prijave na klijente koji nisu u pregledaču, kao što su Outlook, Skype itd, možda ADAL (biblioteka potvrde identiteta Active Directory) nije omogućena na O365 pretplati.</span><span class="sxs-lookup"><span data-stu-id="cced6-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cced6-110">U ovom slučaju moraćete da se povežete sa uslugom Exchange online PowerShell i uradite ovaj cmdlet:  *setu-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*</span><span class="sxs-lookup"><span data-stu-id="cced6-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>