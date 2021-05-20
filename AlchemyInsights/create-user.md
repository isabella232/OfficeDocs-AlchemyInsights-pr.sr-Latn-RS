---
title: Kreiranje korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569761"
---
# <a name="create-user"></a><span data-ttu-id="a675a-102">Kreiranje korisnika</span><span class="sxs-lookup"><span data-stu-id="a675a-102">Create user</span></span>

<span data-ttu-id="a675a-103">**OBJAVA:**</span><span class="sxs-lookup"><span data-stu-id="a675a-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="a675a-104">[Ukidanje podrške za prijavljivanje na WebView iz usluge Google od 4. januara 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="a675a-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="a675a-105">Testirajte da li aplikacija može da utiče tako što ćete pratiti [uputstva](https://go.microsoft.com/fwlink/?linkid=2157323) google za testiranje kompatibilnosti.</span><span class="sxs-lookup"><span data-stu-id="a675a-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="a675a-106">Uverite se da koristite veb pregled sistema ili pregledač sistema kada se prijavljujte korisnicima sa korisničkim Google nalozima.</span><span class="sxs-lookup"><span data-stu-id="a675a-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="a675a-107">Više informacija potražite u [temi Problemi sa prijavljivanjem u aplikacije samo pomoću pregledača Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="a675a-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="a675a-108">**Ne mogu da kreiram novog korisnika u Azure AD direktorijumu**</span><span class="sxs-lookup"><span data-stu-id="a675a-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="a675a-109">Uverite se da ste ovlašćeni za kreiranje novog standardnog korisnika.</span><span class="sxs-lookup"><span data-stu-id="a675a-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="a675a-110">Samo uloga globalnog administratora ili administratora Azure Active Directory (AD) može da kreira novog standardnog korisnika.</span><span class="sxs-lookup"><span data-stu-id="a675a-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="a675a-111">Ako niste u jednoj od ovih uloga, zatražite od administratora da vas doda u jednu od ovih uloga ili da vam kreira novi korisnički nalog.</span><span class="sxs-lookup"><span data-stu-id="a675a-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="a675a-112">Uverite se da se korisničko ime nalazi u domenu koji je verifikovan u vašoj Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a675a-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="a675a-113">Ako nemate verifikovana prilagođena imena domena u Azure AD, možete da koristite početni domen Azure AD koji se završava sa \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="a675a-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="a675a-114">Uverite se da se korisničko ime nalazi u domenu koji nije federan za Azure AD iz vaše bele AD mreže.</span><span class="sxs-lookup"><span data-stu-id="a675a-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="a675a-115">Korisnici ne mogu da se dodaju u oblak sa imenima domena koja su sačinjena iz izvora iz izvora.</span><span class="sxs-lookup"><span data-stu-id="a675a-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="a675a-116">Uverite se da nijedan drugi korisnik ili kontakt već nema korisničko ime koje želite da dodelite novom korisniku.</span><span class="sxs-lookup"><span data-stu-id="a675a-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="a675a-117">Korisnička imena moraju biti jedinstvena u Azure AD- u.</span><span class="sxs-lookup"><span data-stu-id="a675a-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="a675a-118">Pogledajte [Azure AD uloge i administratore](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a675a-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="a675a-119">Pogledajte imena [domena](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a675a-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="a675a-120">Pregledajte [evidenciju nadzora](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) da biste videli detaljnije informacije o nedavno kreiranom ili izbrisanom korisniku kao što su ko je izvršio radnju i kada.</span><span class="sxs-lookup"><span data-stu-id="a675a-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="a675a-121">Više informacija o dodavanju novih korisnika potražite u temi Korišćenje Azure portala za kreiranje novog korisnika [u Azure AD- u](/azure/active-directory/active-directory-users-create-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="a675a-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="a675a-122">[Azure AD administrativne uloge:](/azure/active-directory/active-directory-assign-admin-roles)Administratorske dozvole za uloge u Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a675a-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="a675a-123">Možete da [koristite i Azure AD PowerShell da biste kreirali novog korisnika.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="a675a-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
