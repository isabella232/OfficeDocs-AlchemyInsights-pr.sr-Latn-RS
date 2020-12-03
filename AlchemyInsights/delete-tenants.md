---
title: Brisanje zakupca
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564882"
---
# <a name="delete-tenant"></a><span data-ttu-id="eedb5-102">Brisanje zakupca</span><span class="sxs-lookup"><span data-stu-id="eedb5-102">Delete tenant</span></span>

<span data-ttu-id="eedb5-103">Da biste izbrisali Azure reklamu, obezbedite:</span><span class="sxs-lookup"><span data-stu-id="eedb5-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="eedb5-104">Vi ste globalni administrator u direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="eedb5-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="eedb5-105">Niste prijavljeni pomoću naloga koji ima podrazumevani direktorijum kao što je contoso.onmicrosoft.com na nalogu, kao što je admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="eedb5-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="eedb5-106">Uklonite sve aktivne aplikacije u direktorijumu pre brisanja.</span><span class="sxs-lookup"><span data-stu-id="eedb5-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="eedb5-107">Da biste uklonili aktivne aplikacije, pređite na registraciju aplikacija i uklonite postojeće aplikacije.</span><span class="sxs-lookup"><span data-stu-id="eedb5-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="eedb5-108">Ne postoje aktivne pretplate za bilo koje Microsoft usluge na mreži, kao što je Microsoft Azure, Office 365 ili Azure AD Premium povezane u direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="eedb5-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="eedb5-109">Prebacite pretplate ili ubrzano otkazivanje aktivnih pretplata putem Azure podrške i naplate.</span><span class="sxs-lookup"><span data-stu-id="eedb5-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="eedb5-110">Saznajte više o tome kako da otkažete Office 365 i Azure pretplate.</span><span class="sxs-lookup"><span data-stu-id="eedb5-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="eedb5-111">Za uputstva o asocijaciji ili dodavanju postojeće pretplate zakupcu pogledajte [članak pridruživanje Azure usluzi AZURE AD zakupcu](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="eedb5-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="eedb5-112">Nema aktivne licence.</span><span class="sxs-lookup"><span data-stu-id="eedb5-112">There are no Active license.</span></span> <span data-ttu-id="eedb5-113">Da biste uklonili licence, pogledajte [Kako da uklonite pretplatu da biste uklonili licencu](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="eedb5-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="eedb5-114">Ne postoje drugi aktivni korisnici u direktorijumu osim kada pokušate da izbrišete Azure AD.</span><span class="sxs-lookup"><span data-stu-id="eedb5-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="eedb5-115">Uklonite sve aktivne korisnike i bilo koje zavisnosti od prilagođenog imena domena u zakupcu i treba da se uklone, kao što su korisnici kreirani admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="eedb5-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="eedb5-116">Dodatne detalje o tome kako da:</span><span class="sxs-lookup"><span data-stu-id="eedb5-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="eedb5-117">Izbrišite "Azure Active Directory" ili "pretplata", pogledajte članak [Brisanje Azure aktivnog direktorijuma](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="eedb5-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="eedb5-118">Uklanjanje aplikacija iz direktorijuma potražite u članku [Uklanjanje aplikacija](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="eedb5-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
