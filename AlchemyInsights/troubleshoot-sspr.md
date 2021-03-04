---
title: Rešavanje problema sa SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430216"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="6244e-102">Rešavanje problema sa SSPR</span><span class="sxs-lookup"><span data-stu-id="6244e-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="6244e-103">**Imam problema sa konfigurisanjem poništavanja lozinke**</span><span class="sxs-lookup"><span data-stu-id="6244e-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="6244e-104">Ako ste administrator i tražite kako da omogućite samouslužno poništavanje lozinke, pogledajte [članak uputstvo za omogućavanje SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)da biste konfigurisali poništavanje lozinke za organizaciju.</span><span class="sxs-lookup"><span data-stu-id="6244e-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="6244e-105">Možda ćete želeti da pregledate i [zahteve za licenciranje](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="6244e-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="6244e-106">Morate da imate najmanje jednu licencu dodeljenu u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="6244e-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="6244e-107">**Samo oblaci korisnici** – bilo koji Office 365 (O365) plaćeni MJ ili AZURE AD Basic</span><span class="sxs-lookup"><span data-stu-id="6244e-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="6244e-108">**Cloud i/ili lokalno korisnici** – AZURE AD Premium P1 ili P2, Enterprise mobilnost + Security (Ems) ili bezbedno preduzeće (SPE)</span><span class="sxs-lookup"><span data-stu-id="6244e-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="6244e-109">Za dodatna pitanja o poništavanju lozinke za samouslužno, pregledajte [naša najčešća pitanja](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="6244e-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="6244e-110">**Dobijam poruku o grešci**</span><span class="sxs-lookup"><span data-stu-id="6244e-110">**I'm getting an error message**</span></span>

<span data-ttu-id="6244e-111">Pregledajte ovaj članak da biste pronašli uobičajene greške i njihova rešenja: [Rešavanje problema samouslužnog poništavanja lozinke](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="6244e-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="6244e-112">**Imam problem sa smernicama za poništavanje lozinke**</span><span class="sxs-lookup"><span data-stu-id="6244e-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="6244e-113">Ako se vaša smernica za poništavanje lozinke ne ponaša po očekivanom ili ako imate pitanja o smernicama za poništavanje lozinki, pregledajte ovaj članak: [smernice za lozinke i ograničenja u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="6244e-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="6244e-114">Smernice za poništavanje lozinke se ne primenjuju na administratore.</span><span class="sxs-lookup"><span data-stu-id="6244e-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="6244e-115">Korporacija Microsoft obavezuje podrazumevane smernice za poništavanje lozinke sa dva vrata za bilo koju ulogu usluge Azure.</span><span class="sxs-lookup"><span data-stu-id="6244e-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="6244e-116">Uverite se da testirate sa korisnikom koji nije administrator.</span><span class="sxs-lookup"><span data-stu-id="6244e-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="6244e-117">Više informacija o administratorskim smernicama administratora potražite u članku: administrator je [poništilo razlike u smernicama](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="6244e-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="6244e-118">**Ne želim da moji korisnici registruju dodatne bezbednosne informacije za poništavanje lozinke**</span><span class="sxs-lookup"><span data-stu-id="6244e-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="6244e-119">Možete unapred da popunjavate podatke (e-poštu i telefonske atribute) za korisnike koristeći API, PowerShell ili Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6244e-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="6244e-120">Da biste saznali kako se čita:</span><span class="sxs-lookup"><span data-stu-id="6244e-120">To learn how read:</span></span>

- [<span data-ttu-id="6244e-121">Primena početne vrednosti poništavanja bez potrebe korisnika da se registruju</span><span class="sxs-lookup"><span data-stu-id="6244e-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="6244e-122">Koje podatke koristi poništavanje lozinke</span><span class="sxs-lookup"><span data-stu-id="6244e-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="6244e-123">**Želim da moji korisnici registruju dodatne bezbednosne informacije za poništavanje lozinke**</span><span class="sxs-lookup"><span data-stu-id="6244e-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="6244e-124">Neka vaši korisnici registruju svoje bezbednosne informacije za poništavanje lozinke samouslužavanja tako što ćete ih usmeriti na [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).</span><span class="sxs-lookup"><span data-stu-id="6244e-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="6244e-125">Kada su podaci naseljeni za korisnika (korisnik ili administrator), usmerite korisnika na [aka.MS/sspr](https://passwordreset.microsoftonline.com/) kako bi korisnici mogli da imaju ovlašćenja da ponovo postave sopstvene lozinke.</span><span class="sxs-lookup"><span data-stu-id="6244e-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="6244e-126">Ako korisnici i dalje imaju **problema, oni su najverovatnije automatski** automatski ili **hash sinhronizovanje lozinki** .</span><span class="sxs-lookup"><span data-stu-id="6244e-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="6244e-127">To znači da je verovatno problem sa uslugom poništavanje lozinki.</span><span class="sxs-lookup"><span data-stu-id="6244e-127">This means there is likely a problem with the Password Writeback service.</span></span>