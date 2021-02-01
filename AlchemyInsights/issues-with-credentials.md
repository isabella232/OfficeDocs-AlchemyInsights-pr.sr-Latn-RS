---
title: Problemi sa akreditivima
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063686"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="3a01c-102">Problemi sa akreditivima</span><span class="sxs-lookup"><span data-stu-id="3a01c-102">Issues with credentials</span></span>

<span data-ttu-id="3a01c-103">[Microsoft Platform identiteta i oauth 2,0 pristup akreditivima klijenta](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) opisuje kako se programira direktno sa oauth 2,0 akreditivima klijenata.</span><span class="sxs-lookup"><span data-stu-id="3a01c-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="3a01c-104">**Kako da upravljam lozinkom aplikacije ili akreditivima certifikata?**</span><span class="sxs-lookup"><span data-stu-id="3a01c-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="3a01c-105">U Azure CLI možete da koristite akreditiv [ad App App](https://docs.microsoft.com/cli/azure/ad/app/credential) za brisanje, listu ili resetovanje lozinke aplikacije ili akreditiva certifikata.</span><span class="sxs-lookup"><span data-stu-id="3a01c-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="3a01c-106">**Kako moji korisnici mogu da resetuju lozinke?**</span><span class="sxs-lookup"><span data-stu-id="3a01c-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="3a01c-107">Korisnici treba da se [registruju za samouslužno poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) pre nego što mogu da resetuju lozinke.</span><span class="sxs-lookup"><span data-stu-id="3a01c-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="3a01c-108">Kada se korisnik registruje, oni mogu da slede uputstva iz ovog članka da bi poništili svoju lozinku: [poništili lozinku za posao ili školu](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span><span class="sxs-lookup"><span data-stu-id="3a01c-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="3a01c-109">**Kako korisnici menjaju lozinke?**</span><span class="sxs-lookup"><span data-stu-id="3a01c-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="3a01c-110">Korisnici mogu da slede korake iz ovog članka da bi promenili lozinke: [Kako da promenite lozinku](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span><span class="sxs-lookup"><span data-stu-id="3a01c-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="3a01c-111">Takođe mogu da [upravljaju lozinkama za aplikacije iz dva koraka](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span><span class="sxs-lookup"><span data-stu-id="3a01c-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="3a01c-112">**Moj korisnik dobija grešku prilikom promene ili ponovnog podešavanja lozinke**</span><span class="sxs-lookup"><span data-stu-id="3a01c-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="3a01c-113">Ova karika će pružiti informacije o uobičajenim problemima koji mogu da se pojave kada korisnik pokušava da poništi lozinku: [uobičajeni problemi i rešenja](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="3a01c-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="3a01c-114">**Imam problem sa ponovnim postavljanjem lozinke korisnika**</span><span class="sxs-lookup"><span data-stu-id="3a01c-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="3a01c-115">Proverite da li ste ovlašćeni za poništavanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="3a01c-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="3a01c-116">*Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.*</span><span class="sxs-lookup"><span data-stu-id="3a01c-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3a01c-117">Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.</span><span class="sxs-lookup"><span data-stu-id="3a01c-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="3a01c-118">Uverite se da ste razumeli zahteve licenciranja:</span><span class="sxs-lookup"><span data-stu-id="3a01c-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="3a01c-119">Morate imati bar jednu licencu dodeljenu u organizaciji:</span><span class="sxs-lookup"><span data-stu-id="3a01c-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="3a01c-120">**Samo oblaci korisnici** – bilo koji Office 365 (O365) plaćeni MJ ili AZURE AD Basic</span><span class="sxs-lookup"><span data-stu-id="3a01c-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="3a01c-121">**Cloud i/ili lokalno korisnici** – AZURE AD Premium P1 ili P2, Enterprise mobilnost + Security (Ems) ili bezbedno preduzeće (SPE)</span><span class="sxs-lookup"><span data-stu-id="3a01c-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="3a01c-122">Da biste saznali više o zahtevima licenciranja, pogledajte članak [licenciranje zahteva za pretraživanje lozinke za Azure AD samouslužno](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span><span class="sxs-lookup"><span data-stu-id="3a01c-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="3a01c-123">Da biste poništili lozinku korisnika, pronađite korisnika u usluzi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3a01c-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="3a01c-124">Zatim, na oštrici za taj korisnik kliknite na dugme "poništi lozinku".</span><span class="sxs-lookup"><span data-stu-id="3a01c-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="3a01c-125">**Dugme "poništi lozinku" je premačeno**</span><span class="sxs-lookup"><span data-stu-id="3a01c-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="3a01c-126">Nemate dozvolu da poništite lozinke **ovog** korisnika.</span><span class="sxs-lookup"><span data-stu-id="3a01c-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="3a01c-127">*Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.*</span><span class="sxs-lookup"><span data-stu-id="3a01c-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3a01c-128">Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.</span><span class="sxs-lookup"><span data-stu-id="3a01c-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3a01c-129">**Ne vidim nož za poništavanje lozinke**</span><span class="sxs-lookup"><span data-stu-id="3a01c-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="3a01c-130">Nemate dozvolu da poništite lozinke.</span><span class="sxs-lookup"><span data-stu-id="3a01c-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="3a01c-131">*Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.*</span><span class="sxs-lookup"><span data-stu-id="3a01c-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3a01c-132">Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.</span><span class="sxs-lookup"><span data-stu-id="3a01c-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3a01c-133">**Ne mogu da vidim lokalnu oљtricu za integraciju u polju za poništavanje lozinke**</span><span class="sxs-lookup"><span data-stu-id="3a01c-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="3a01c-134">Oљtrica lokalno integracije se pojavljuje samo u hibridne okruženja – što znači da koristite ispravnu lozinku za manipulisanje lozinkama korisnika.</span><span class="sxs-lookup"><span data-stu-id="3a01c-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="3a01c-135">Ne vidite ovaj nož ako:</span><span class="sxs-lookup"><span data-stu-id="3a01c-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="3a01c-136">Ne koristite ponovno upisivanje lozinki</span><span class="sxs-lookup"><span data-stu-id="3a01c-136">You are not using password writeback</span></span>
  - <span data-ttu-id="3a01c-137">Postoji problem sa instalacijom/povezivanjem lozinke za poništavanje lozinki</span><span class="sxs-lookup"><span data-stu-id="3a01c-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="3a01c-138">Postoji problem sa instalacijom/povezivanjem Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="3a01c-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="3a01c-139">Više koraka za rešavanje problema sa lozinkama pri vraćanju lozinki potražite u članku [Rešavanje problema sa lozinkom ponovno upisivanje](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="3a01c-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="3a01c-140">**Ne znam kako da poništim lozinku korisnika**</span><span class="sxs-lookup"><span data-stu-id="3a01c-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="3a01c-141">Prijavite se na Azure portal kao odgovarajući administrator.</span><span class="sxs-lookup"><span data-stu-id="3a01c-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="3a01c-142">Idite na Blade za **korisnike i grupe** , izaberite stavku **Svi korisnici**.</span><span class="sxs-lookup"><span data-stu-id="3a01c-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="3a01c-143">Izaberite korisnika sa liste.</span><span class="sxs-lookup"><span data-stu-id="3a01c-143">Select a user from the list.</span></span>
4. <span data-ttu-id="3a01c-144">Za izabranog korisnika, izaberite stavku **Pregled**, a zatim na komandnoj traci izaberite stavku **Poništi lozinku**.</span><span class="sxs-lookup"><span data-stu-id="3a01c-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="3a01c-145">Kliknite na dugme **Poništi lozinku** i uradite uputstva na ekranu.</span><span class="sxs-lookup"><span data-stu-id="3a01c-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="3a01c-146">Samo resetima koji se izvršavaju putem **Azure portala** podržavaju ponovno upisivanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="3a01c-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="3a01c-147">**Resetovao sam lozinku lokalnog korisnika sa Office 365 portala administracije ili Office 365 mobilnog aplikacije, ali korisnik i dalje ne može da se prijavi**</span><span class="sxs-lookup"><span data-stu-id="3a01c-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="3a01c-148">Povratni lozinku nije podržan na ovom portalu.</span><span class="sxs-lookup"><span data-stu-id="3a01c-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="3a01c-149">Ponovo uspostavite lozinku korisnika na Azure portalu.</span><span class="sxs-lookup"><span data-stu-id="3a01c-149">Reset the user's password again in the Azure portal.</span></span>
