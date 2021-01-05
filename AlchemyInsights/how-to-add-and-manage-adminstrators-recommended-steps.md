---
title: Kako se dodaju i upravljaju administratorima koji se preporučuju
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755849"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="a7939-102">Kako se dodaju i upravljaju administratorima koji se preporučuju</span><span class="sxs-lookup"><span data-stu-id="a7939-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="a7939-103">Na osnovu opisa problema, našli smo rešenje za vas.</span><span class="sxs-lookup"><span data-stu-id="a7939-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="a7939-104">Većina klijenata mogla je samostalno da rešava svoj problem nakon praćenja dokumentacije.</span><span class="sxs-lookup"><span data-stu-id="a7939-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="a7939-105">**Uređivanje administratora pretplate ili Koadministratora**</span><span class="sxs-lookup"><span data-stu-id="a7939-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="a7939-106">Administrator naloga može da uredi obe uloge dok administrator pretplate može da promeni samo Koadministratore na [Azure portal](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="a7939-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="a7939-107">Dodavanje ili promena Azure administratora pretplate</span><span class="sxs-lookup"><span data-stu-id="a7939-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="a7939-108">**Ažuriranje administratora pretplate ili Co-Administrator za interne (EMITNE) pretplate**</span><span class="sxs-lookup"><span data-stu-id="a7939-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="a7939-109">Administrator usluge ili koadministrator može samouslužiti ovu radnju pomoću sledećih koraka:</span><span class="sxs-lookup"><span data-stu-id="a7939-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="a7939-110">Prijavite se na [Azure portal](https://ms.portal.azure.com/#home) i izaberite stavku **Upravljanje troškovima + naplata** u levom Blejku.</span><span class="sxs-lookup"><span data-stu-id="a7939-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="a7939-111">Kliknite na stavku predmeta sa pretplatom.</span><span class="sxs-lookup"><span data-stu-id="a7939-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="a7939-112">Otvoriće se pregled pretplate.</span><span class="sxs-lookup"><span data-stu-id="a7939-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="a7939-113">Na oštrici **pretplate** kliknite na dugme **Svojstva**.</span><span class="sxs-lookup"><span data-stu-id="a7939-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="a7939-114">Kliknite na dugme **administratora usluge** .</span><span class="sxs-lookup"><span data-stu-id="a7939-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="a7939-115">Unesite e-poruku korisnika koju želite da postaviљ kao administrator usluge i kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="a7939-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="a7939-116">**Dodavanje/promena/uklanjanje Koadministratora**</span><span class="sxs-lookup"><span data-stu-id="a7939-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="a7939-117">Prijavite se na [Azure portal](https://ms.portal.azure.com/#home) kao administrator usluge.</span><span class="sxs-lookup"><span data-stu-id="a7939-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="a7939-118">Otvorite [pretplate](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) i izaberite pretplatu.</span><span class="sxs-lookup"><span data-stu-id="a7939-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="a7939-119">(Saradnici se mogu dodeliti samo na nivou pretplate.)</span><span class="sxs-lookup"><span data-stu-id="a7939-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="a7939-120">Pređite na **Access Control (iam)**  >  **Classic administratori**  >  **dodaju**  >  **programski koadministrator** da bi otvorili okno " **Dodavanje koadministracije** " (ako je opcija "Dodaj koadministrator" onemogućiti, označava da nemate dozvole).</span><span class="sxs-lookup"><span data-stu-id="a7939-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="a7939-121">Izaberite korisnika kojeg želite da dodate i kliknite na dugme **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="a7939-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="a7939-122">**uči više:**</span><span class="sxs-lookup"><span data-stu-id="a7939-122">**Learn more:**</span></span>
- [<span data-ttu-id="a7939-123">Dodavanje Koadministratora</span><span class="sxs-lookup"><span data-stu-id="a7939-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a7939-124">Uklanjanje koadministratora</span><span class="sxs-lookup"><span data-stu-id="a7939-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a7939-125">Promena administratora usluge</span><span class="sxs-lookup"><span data-stu-id="a7939-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a7939-126">Prikaz administratora naloga</span><span class="sxs-lookup"><span data-stu-id="a7939-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="a7939-127">Upravljanje pristupom koristeći RBAC i Azure portal</span><span class="sxs-lookup"><span data-stu-id="a7939-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="a7939-128">**Dodavanje/brisanje korisnika pomoću usluge Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="a7939-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="a7939-129">Možete da dodate nove korisnike ili da izbrišete postojeće korisnike iz usluge Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="a7939-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="a7939-130">Da biste dodali novog korisnika, prijavite se na [Azure portal](https://ms.portal.azure.com/#home) kao korisnički administrator za organizaciju.</span><span class="sxs-lookup"><span data-stu-id="a7939-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="a7939-131">Izaberite stavku **Azure Active Directory**, izaberite stavku **Korisnici** , a zatim stavku **novi korisnik**.</span><span class="sxs-lookup"><span data-stu-id="a7939-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="a7939-132">Na stranici **korisnik** popunite potrebne informacije.</span><span class="sxs-lookup"><span data-stu-id="a7939-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="a7939-133">Kliknite na dugme **Kreiraj**.</span><span class="sxs-lookup"><span data-stu-id="a7939-133">Click **Create**.</span></span> <span data-ttu-id="a7939-134">Korisnik se kreira i dodaje u vaš Azure AD stanar.</span><span class="sxs-lookup"><span data-stu-id="a7939-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="a7939-135">**Saznajte više**:</span><span class="sxs-lookup"><span data-stu-id="a7939-135">**Learn more**:</span></span>

- [<span data-ttu-id="a7939-136">Dodavanje novog korisnika</span><span class="sxs-lookup"><span data-stu-id="a7939-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="a7939-137">Brisanje korisnika</span><span class="sxs-lookup"><span data-stu-id="a7939-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="a7939-138">Dodavanje ili ažuriranje informacija o profilu pomoću usluge Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a7939-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="a7939-139">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="a7939-139">**Recommended documents**</span></span>

- [<span data-ttu-id="a7939-140">Šta je to Kontrola pristupa zasnovan na ulozi (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="a7939-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="a7939-141">Razumevanje raznih uloga u Azure</span><span class="sxs-lookup"><span data-stu-id="a7939-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="a7939-142">Dozvole za administratorske uloge u usluzi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a7939-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="a7939-143">Uputstvo: dodelite pristup korisniku koji koristi RBAC i Azure portal</span><span class="sxs-lookup"><span data-stu-id="a7939-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="a7939-144">Rešavanje problema sa RBAC u Azure</span><span class="sxs-lookup"><span data-stu-id="a7939-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="a7939-145">Organizovanje resursa pomoću usluge Azure Management</span><span class="sxs-lookup"><span data-stu-id="a7939-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="a7939-146">Kako tražiti kopiju Azure fakture putem e-pošte</span><span class="sxs-lookup"><span data-stu-id="a7939-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="a7939-147">Kako da dodate, ažurirate ili uklonite kreditnu ili debitnu karticu sa lokacije Azure</span><span class="sxs-lookup"><span data-stu-id="a7939-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="a7939-148">Upravljanje pretplatom (ponovo Aktiviraj/Otkaži/zameni)</span><span class="sxs-lookup"><span data-stu-id="a7939-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



