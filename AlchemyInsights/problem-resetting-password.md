---
title: Problem pri ponovnom podešavanju lozinke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696276"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="071d6-102">Problemi pri ponovnom podešavanju lozinke</span><span class="sxs-lookup"><span data-stu-id="071d6-102">Problems resetting password</span></span>

<span data-ttu-id="071d6-103">Slede neki od problema sa kojima možete da se suoиite prilikom ponovnog podešavanja lozinke i mogućih rešenja:</span><span class="sxs-lookup"><span data-stu-id="071d6-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="071d6-104">**Imam problem sa poništavanju lozinke koje nisu obuhvaćene drugim kategorijama**</span><span class="sxs-lookup"><span data-stu-id="071d6-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="071d6-105">Uverite se da ste ovlašćeni za poništavanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="071d6-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="071d6-106">Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.</span><span class="sxs-lookup"><span data-stu-id="071d6-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="071d6-107">Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.</span><span class="sxs-lookup"><span data-stu-id="071d6-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="071d6-108">Uverite se da razumete zahteve licenciranja:</span><span class="sxs-lookup"><span data-stu-id="071d6-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="071d6-109">Morate imati bar jednu licencu dodeljenu u organizaciji</span><span class="sxs-lookup"><span data-stu-id="071d6-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="071d6-110">Samo oblaci korisnici – bilo koji Office 365 (O365) plaćeni MJ ili Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="071d6-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="071d6-111">Cloud i/ili lokalno korisnici – Azure AD Premium P1 ili P2, Enterprise mobilnost + Security (EMS) ili bezbedno preduzeće (SPE)</span><span class="sxs-lookup"><span data-stu-id="071d6-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="071d6-112">Da biste pročitali više o zahtevima licenciranja pogledajte [zahteve za licenciranje članaka za Azure AD samouslužno poništavanje lozinke](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="071d6-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="071d6-113">**Imam problema sa ispitivanjem smernica za poništavanje lozinke koju sam podesio**</span><span class="sxs-lookup"><span data-stu-id="071d6-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="071d6-114">Nedavno zatvorene smernice mogu potrajati nekoliko minuta radi replikaciju u svim centrima podataka i krajnjim tačkama.</span><span class="sxs-lookup"><span data-stu-id="071d6-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="071d6-115">Fizički razdaljina iz centra za podatke će takođe uticati na primenu primene promena.</span><span class="sxs-lookup"><span data-stu-id="071d6-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="071d6-116">Testiranje sa krajnjim korisnikom, ne administratorom i pilotu sa malim skupom korisnika.</span><span class="sxs-lookup"><span data-stu-id="071d6-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="071d6-117">Smernice podešene na Azure portovi primenjuju se samo na krajnje korisnike, ne na administratore.</span><span class="sxs-lookup"><span data-stu-id="071d6-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="071d6-118">Microsoft obavezuje podrazumevane smernice za poništavanje lozinke sa dve kapije za bilo koju Azure administratorsku ulogu (primer: globalni administrator, HelpDesk administrator, administrator lozinki itd.)</span><span class="sxs-lookup"><span data-stu-id="071d6-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="071d6-119">Saznajte više o [smernicama za administratore](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="071d6-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="071d6-120">**Želim da pokrenem poništavanje lozinke, ali ne želim da moji korisnici registruju dodatne bezbednosne informacije**</span><span class="sxs-lookup"><span data-stu-id="071d6-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="071d6-121">Unapred popunjavate podatke za korisnike tako da ne moraju!</span><span class="sxs-lookup"><span data-stu-id="071d6-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="071d6-122">-Kao administrator možete da postavite svojstva telefona i e-pošte za korisnike pre nego što izazovete poništavanje lozinki na organizaciju.</span><span class="sxs-lookup"><span data-stu-id="071d6-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="071d6-123">To možete da uradite koristeći API, PowerShell ili Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="071d6-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="071d6-124">Više informacija potražite u člancima:</span><span class="sxs-lookup"><span data-stu-id="071d6-124">More information here:</span></span>
- [<span data-ttu-id="071d6-125">Primena početne vrednosti poništavanja bez potrebe korisnika da se registruju</span><span class="sxs-lookup"><span data-stu-id="071d6-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="071d6-126">Koje podatke koristi poništavanje lozinke</span><span class="sxs-lookup"><span data-stu-id="071d6-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="071d6-127">**Dugme "poništi lozinku" je premačeno**</span><span class="sxs-lookup"><span data-stu-id="071d6-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="071d6-128">Nemate dozvolu da poništite lozinke ovog korisnika.</span><span class="sxs-lookup"><span data-stu-id="071d6-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="071d6-129">Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.</span><span class="sxs-lookup"><span data-stu-id="071d6-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="071d6-130">Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.</span><span class="sxs-lookup"><span data-stu-id="071d6-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="071d6-131">**Ne vidim nož za poništavanje lozinke**</span><span class="sxs-lookup"><span data-stu-id="071d6-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="071d6-132">Nemate dozvolu da poništite lozinke.</span><span class="sxs-lookup"><span data-stu-id="071d6-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="071d6-133">Samo globalna, lozinka i administratori administratora mogu da resetuju korisničke lozinke.</span><span class="sxs-lookup"><span data-stu-id="071d6-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="071d6-134">Globalni administratori mogu da resetuju i druge privilegovane administratorske lozinke.</span><span class="sxs-lookup"><span data-stu-id="071d6-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="071d6-135">**Ne mogu da vidim lokalnu oљtricu za integraciju u polju za poništavanje lozinke**</span><span class="sxs-lookup"><span data-stu-id="071d6-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="071d6-136">Oљtrica lokalno integracije se pojavljuje samo u hibridne okruženja – što znači da koristite ispravnu lozinku za manipulisanje lozinkama korisnika.</span><span class="sxs-lookup"><span data-stu-id="071d6-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="071d6-137">Ne vidite ovaj nož ako:</span><span class="sxs-lookup"><span data-stu-id="071d6-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="071d6-138">Ne koristite ponovno upisivanje lozinki</span><span class="sxs-lookup"><span data-stu-id="071d6-138">You are not using password writeback</span></span>
    - <span data-ttu-id="071d6-139">Postoji problem sa instalacijom/povezivanjem lozinke za poništavanje lozinki</span><span class="sxs-lookup"><span data-stu-id="071d6-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="071d6-140">Postoji problem sa instalacijom/povezivanjem Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="071d6-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="071d6-141">Više koraka za rešavanje problema sa lozinkama pri vraćanju lozinki potražite u odeljku [Rešavanje problema sa lozinkom](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support) ispravkom</span><span class="sxs-lookup"><span data-stu-id="071d6-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="071d6-142">**Ne znam kako da poništim lozinku korisnika**</span><span class="sxs-lookup"><span data-stu-id="071d6-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="071d6-143">Prijavite se na Azure portal kao odgovarajući administrator.</span><span class="sxs-lookup"><span data-stu-id="071d6-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="071d6-144">Idite na Blade za korisnike i grupe, izaberite stavku **Svi korisnici**.</span><span class="sxs-lookup"><span data-stu-id="071d6-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="071d6-145">Izaberite korisnika sa liste.</span><span class="sxs-lookup"><span data-stu-id="071d6-145">Select a user from the list.</span></span>
1. <span data-ttu-id="071d6-146">Za izabranog korisnika, izaberite stavku **Pregled**, a zatim na komandnoj traci kliknite na dugme **Poništi lozinku**.</span><span class="sxs-lookup"><span data-stu-id="071d6-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="071d6-147">Izvršite uputstva na ekranu.</span><span class="sxs-lookup"><span data-stu-id="071d6-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="071d6-148">Samo resetima koji se izvršavaju putem Azure portala podržavaju ponovno upisivanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="071d6-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="071d6-149">**Resetovao sam lozinku lokalnog korisnika sa Office 365 portala administracije ili Office 365 mobilnog aplikacije, ali korisnik i dalje ne može da se prijavi**</span><span class="sxs-lookup"><span data-stu-id="071d6-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="071d6-150">Povratni lozinku nije podržan na ovom portalu.</span><span class="sxs-lookup"><span data-stu-id="071d6-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="071d6-151">Ponovo poništite lozinku korisnika u Azure portalu – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="071d6-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

