---
title: Migracija iz programa AIP u MIP/ujedinjavanje u centru za usaglašenost
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674340"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="2a060-102">Migracija iz programa AIP u MIP/ujedinjavanje u centru za usaglašenost</span><span class="sxs-lookup"><span data-stu-id="2a060-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="2a060-103">Da biste migrirali sa AIP nalepnica do jedinstvenog označavanja u centru za bezbednost i usaglašenost, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="2a060-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="2a060-104">**Aktivacija zaštite sa Azure portala**</span><span class="sxs-lookup"><span data-stu-id="2a060-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="2a060-105">Ako to već niste uradili, otvorite novi prozor pregledača i [Prijavite se na Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="2a060-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="2a060-106">Pređite na oљtricu **Azure zaštite informacija** .</span><span class="sxs-lookup"><span data-stu-id="2a060-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="2a060-107">Na primer, u meniju čvorište izaberite stavku **sve usluge** i počnite da kucate **informacije** u polju Filter.</span><span class="sxs-lookup"><span data-stu-id="2a060-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="2a060-108">Izaberite stavku **Azure zaštita informacija**.</span><span class="sxs-lookup"><span data-stu-id="2a060-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="2a060-109">Ako niste ranije pristupili Azure zaštiti informacija, pogledajte sledeće [korake](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) da biste dodali ovu oљtricu na portal.</span><span class="sxs-lookup"><span data-stu-id="2a060-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="2a060-110">Da biste otvorili karticu Azure zaštite informacija, morate imati ili [Azure Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ili Office 365 plan koji uključuje upravljanje pravima.</span><span class="sxs-lookup"><span data-stu-id="2a060-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="2a060-111">Ako imate jednu od ovih pretplata, ali vidite poruku da nije moguće pronaći važeću pretplatu, obratite se [Microsoft podršci](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ili koristite standardne kanale podrške.</span><span class="sxs-lookup"><span data-stu-id="2a060-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="2a060-112">Pronađite opcije **upravljanja** menijima i izaberite stavku **aktivacija zaštite**.</span><span class="sxs-lookup"><span data-stu-id="2a060-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="2a060-113">Kliknite na dugme **Aktiviraj**, a zatim potvrdite radnju.</span><span class="sxs-lookup"><span data-stu-id="2a060-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="2a060-114">Kada se aktivacija dovrši, informativna traka prikazuje **Aktiviranje je završeno**.</span><span class="sxs-lookup"><span data-stu-id="2a060-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="2a060-115">**Migriranje Azure usluge zaštite informacija u Office 365 Security & centar za usaglašenost**</span><span class="sxs-lookup"><span data-stu-id="2a060-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="2a060-116">Uverite se da ste prijavljeni kao korisnik sa dozvolom globalnog administratora.</span><span class="sxs-lookup"><span data-stu-id="2a060-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="2a060-117">Pređite na oљtricu **Azure zaštite informacija** .</span><span class="sxs-lookup"><span data-stu-id="2a060-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="2a060-118">U opciji **Upravljanje** menijima izaberite stavku **objedinjeno označavanje**.</span><span class="sxs-lookup"><span data-stu-id="2a060-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="2a060-119">Na **sečivu Azure informacije – objedinjeno označavanje informacija** kliknite na dugme **Aktiviraj** i sledi uputstva na mreži.</span><span class="sxs-lookup"><span data-stu-id="2a060-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="2a060-120">**Napomena**: proverite da li imate odgovarajuće dozvole pre nego što aktivirate migraciju centra za usaglašenost &.</span><span class="sxs-lookup"><span data-stu-id="2a060-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="2a060-121">Pogledajte ove članke za više informacija:</span><span class="sxs-lookup"><span data-stu-id="2a060-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="2a060-122">Da li treba da budete globalni administrator da biste konfigurisali Azure zaštitu informacija ili mogu da delegat drugim administratorima?</span><span class="sxs-lookup"><span data-stu-id="2a060-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="2a060-123">Važne informacije o administratorskim ulogama posle migriranja u bezbednosni & centru za usaglašenost.</span><span class="sxs-lookup"><span data-stu-id="2a060-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="2a060-124">Više informacija o AIP-u za Ujedinjeno označavanje migracije u centar za bezbednost i usaglašenost potražite u članku [Migriranje nalepnica](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="2a060-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
