---
title: Rešavanje problema sa savršenim prijavljivanjem zasnovanim na lozinkama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714885"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="5aa20-102">Rešavanje problema sa savršenim prijavljivanjem zasnovanim na lozinkama</span><span class="sxs-lookup"><span data-stu-id="5aa20-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="5aa20-103">Da biste naučili osnove SSO lozinki, pogledajte članak [potvrda identiteta zasnovanu na lozinci sa uslugom Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="5aa20-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="5aa20-104">**Konfigurisanje SSO-a zasnovan na lozinci**</span><span class="sxs-lookup"><span data-stu-id="5aa20-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="5aa20-105">[Konfigurisanje jedinstvenog prijavljivanja na zasnovan na lozinci](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -ovaj članak sadrži detaljnije informacije o opciji SSO na osnovu lozinke.</span><span class="sxs-lookup"><span data-stu-id="5aa20-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="5aa20-106">Ako aplikacija koju dodajete zahteva prilagođenu konfiguraciju i morate da koristite SSO na osnovu lozinki, ovaj članak je za vas.</span><span class="sxs-lookup"><span data-stu-id="5aa20-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="5aa20-107">[Konfigurisanje jedinstvenog prijavljivanja na zasnovan na lozinci za aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) "</span><span class="sxs-lookup"><span data-stu-id="5aa20-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="5aa20-108">Prijavljivanje zasnovano na lozinci je namenjeno aplikacijama koje koriste kombinaciju korisničkog imena/lozinki za potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="5aa20-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="5aa20-109">Kada konfigurišete prijavljivanje na osnovu lozinki za aplikaciju, korisnici moraju da se prijave u lokalnu aplikaciju jednom.</span><span class="sxs-lookup"><span data-stu-id="5aa20-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="5aa20-110">Posle toga, Azure Active Directory skladišti informacije za prijavljivanje i automatski je pruža aplikaciji kada korisnici pristupe daljinski.</span><span class="sxs-lookup"><span data-stu-id="5aa20-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="5aa20-111">Trebalo je da objavite i testirate aplikaciju sa proxy serverom.</span><span class="sxs-lookup"><span data-stu-id="5aa20-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="5aa20-112">Ako to ne uradite, slijedite korake u odeljku [objavljivanje aplikacija pomoću usluge Azure AD Application proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application)</span><span class="sxs-lookup"><span data-stu-id="5aa20-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="5aa20-113">Da biste rešili problem sa lozinkom zasnovanim na lozinci, pogledajte članak [Rešavanje problema sa jedinstvenim prijavljivanjem zasnovanim na lozinci](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="5aa20-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
