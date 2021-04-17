---
title: Migracija iz AIP u MIP/unified Labeling u centru za usaglašenost
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825385"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="88cb0-102">Migracija iz AIP u MIP/unified Labeling u centru za usaglašenost</span><span class="sxs-lookup"><span data-stu-id="88cb0-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="88cb0-103">Da biste migrirani iz AIP nalepnica u "Ujedinjeno označavanje" u centru za bezbednost i usaglašenost, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="88cb0-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="88cb0-104">**Aktiviranje zaštite sa Azure portala**</span><span class="sxs-lookup"><span data-stu-id="88cb0-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="88cb0-105">Ako to već niste uradili, otvorite novi prozor pregledača i [prijavite se na Azure portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="88cb0-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="88cb0-106">Prešli na **Azure Information Protection** blejd.</span><span class="sxs-lookup"><span data-stu-id="88cb0-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="88cb0-107">Na primer, u meniju Čvorište izaberite stavku **Sve usluge** i počnite da kucate **informacije** u polju Filter.</span><span class="sxs-lookup"><span data-stu-id="88cb0-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="88cb0-108">Izaberite **stavku Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="88cb0-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="88cb0-109">Ako ranije niste pristupili Azure Information Protection bleju, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) pogledajte jedno vreme dodatne korake da biste dodali ovaj blejd na portal.</span><span class="sxs-lookup"><span data-stu-id="88cb0-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="88cb0-110">Da biste otvorili Azure Information Protection blejd, morate da imate [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ili Office 365 plan koji obuhvata Rights Management.</span><span class="sxs-lookup"><span data-stu-id="88cb0-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="88cb0-111">Ako imate jednu od ovih pretplata, ali vidite poruku da nije moguće pronaći važeću pretplatu, obratite se [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) podršci ili koristite standardne kanale podrške.</span><span class="sxs-lookup"><span data-stu-id="88cb0-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="88cb0-112">Pronađite **opcije menija** "Upravljanje" i izaberite **stavku Aktivacija zaštite.**</span><span class="sxs-lookup"><span data-stu-id="88cb0-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="88cb0-113">Kliknite na **aktiviranje**, a zatim potvrdite radnju.</span><span class="sxs-lookup"><span data-stu-id="88cb0-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="88cb0-114">Kada se aktivacija dovrši, traka sa informacijama prikazuje **da je Aktivacija uspešno završena.**</span><span class="sxs-lookup"><span data-stu-id="88cb0-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="88cb0-115">**Migracija Azure Information Protection oznaka u Office 365 centar za & usaglašenost**</span><span class="sxs-lookup"><span data-stu-id="88cb0-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="88cb0-116">Proverite da li ste prijavljeni kao korisnik sa dozvolom globalnog administratora.</span><span class="sxs-lookup"><span data-stu-id="88cb0-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="88cb0-117">Prešli na **Azure Information Protection** blejd.</span><span class="sxs-lookup"><span data-stu-id="88cb0-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="88cb0-118">U opciji **menija** Upravljanje izaberite stavku **"Ujedinjena oznaka"**.</span><span class="sxs-lookup"><span data-stu-id="88cb0-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="88cb0-119">Na **bleju Azure Information Protection – unified labeling** blade kliknite na **Aktiviraj** i pratite uputstva na mreži.</span><span class="sxs-lookup"><span data-stu-id="88cb0-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="88cb0-120">**Na primer: Uverite** se da imate odgovarajuće dozvole pre aktivacije migracije centra za & usaglašenost centra za usaglašenost.</span><span class="sxs-lookup"><span data-stu-id="88cb0-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="88cb0-121">Pogledajte ove članke za više informacija:</span><span class="sxs-lookup"><span data-stu-id="88cb0-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="88cb0-122">Da li treba da budete globalni administrator da biste konfigurisali Azure Information Protection ili mogu da delegiram drugim administratorima?</span><span class="sxs-lookup"><span data-stu-id="88cb0-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="88cb0-123">Važne informacije o administrativnim ulogama posle migracije u centar & za usaglašenost.</span><span class="sxs-lookup"><span data-stu-id="88cb0-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="88cb0-124">Dodatne informacije o migraciji AIP-a u centar za bezbednost i usaglašenost potražite u temi [Migracija nalepnica.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="88cb0-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
