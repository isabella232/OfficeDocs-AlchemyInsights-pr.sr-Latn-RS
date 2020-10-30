---
title: Pristup pretplate
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807720"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="ff797-102">Nije moguće prijaviti Azure za prijavljivanje zbog problema sa pregledom (pregledač se ne odaziva, nastavlja da se vrti, ne učita itd.)</span><span class="sxs-lookup"><span data-stu-id="ff797-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="ff797-103">Možda ćete imati problema sa nestankom.</span><span class="sxs-lookup"><span data-stu-id="ff797-103">You might be impacted by an outage.</span></span> <span data-ttu-id="ff797-104">Proverite da li postoji trenutna nestanka: [Azure zdravstveni status](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="ff797-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="ff797-105">Odjavite se sa svih aktivnih Azure sesija.</span><span class="sxs-lookup"><span data-stu-id="ff797-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="ff797-106">Započnite privatno ili inkognito režim Veb pregledača.</span><span class="sxs-lookup"><span data-stu-id="ff797-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="ff797-107">Možete i da pokušate da osvežite pregledač, koristite drugi pregledač, izbrišete keš keširanja ako iznad ne funkcioniše.</span><span class="sxs-lookup"><span data-stu-id="ff797-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="ff797-108">Saznajte više: [Rešavanje problema sa prijavljivanjem](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="ff797-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="ff797-109">**Nije moguće pristupiti pretplatama**</span><span class="sxs-lookup"><span data-stu-id="ff797-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="ff797-110">Na sajtu [Azure](https://portal.azure.com/)uverite se da je u nalogu u gornjem desnom članku izabrana Azure direktorijum.</span><span class="sxs-lookup"><span data-stu-id="ff797-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="ff797-111">U [centru Azure naloga](https://account.windowsazure.com/Subscriptions)proverite da li je nalog koji se koristi administrator naloga.</span><span class="sxs-lookup"><span data-stu-id="ff797-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="ff797-112">Saznajte više: [Rešavanje problema sa pronađenih pretplata](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ff797-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="ff797-113">**Nije moguće pristupiti istoriji naplata**</span><span class="sxs-lookup"><span data-stu-id="ff797-113">**Unable to access billing history**</span></span>

<span data-ttu-id="ff797-114">Administrator naloga mora da se uveri da se korisnik pristupa informacijama o naplati dodaje u Azure Active Directory kao korisnik gosta: [Dodavanje ili brisanje novog korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ff797-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ff797-115">Korisniku treba da se dodeli globalna uloga administratora: [Dodeli ulogu korisnicima](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ff797-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ff797-116">Proknjižite ovo, korisniku može biti dat pristup naplate koristeći RBAC smernice: [Dodeli pristup naplata](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ff797-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ff797-117">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="ff797-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="ff797-118">Ne mogu da se prijavim za upravljanje Azure pretplatom</span><span class="sxs-lookup"><span data-stu-id="ff797-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)