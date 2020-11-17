---
title: Privilegija upravljanja identitetom
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089153"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="1c154-102">Privilegija za upravljanje identitetom (PIM)</span><span class="sxs-lookup"><span data-stu-id="1c154-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="1c154-103">**Dozvole se ne odobravaju nakon aktiviranja uloge**</span><span class="sxs-lookup"><span data-stu-id="1c154-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="1c154-104">Kada aktivirate ulogu u usluzi Azure A.D. za upravljanje identitetom (PIM), aktivacija se možda neće odmah preneti na sve portove koji zahtevaju privilegovanu ulogu.</span><span class="sxs-lookup"><span data-stu-id="1c154-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="1c154-105">Ponekad, čak i ako se promena produži, Veb keširanje na portalu može dovesti do toga da promena ne stupa na snagu odmah.</span><span class="sxs-lookup"><span data-stu-id="1c154-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="1c154-106">Ako je aktivacija odložena, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="1c154-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="1c154-107">Odjavite se sa Azure portala, a zatim se ponovo prijavite.</span><span class="sxs-lookup"><span data-stu-id="1c154-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="1c154-108">Kada aktivirate Azure reklamu uloge ili vrednost Azure resursa, videćete faze aktivacije.</span><span class="sxs-lookup"><span data-stu-id="1c154-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="1c154-109">Kada se sve faze završe, videćete povezanost "odjavljivanje".</span><span class="sxs-lookup"><span data-stu-id="1c154-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="1c154-110">Možete da koristite ovu povezanost da biste se odjavili. Ovo će rešiti većinu slučajeva za odlaganje aktiviranja.</span><span class="sxs-lookup"><span data-stu-id="1c154-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="1c154-111">U okviru PIM, proverite da li ste navedeni kao član uloge.</span><span class="sxs-lookup"><span data-stu-id="1c154-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="1c154-112">Ako aktivirate ulogu administratora Exchange servera, obavezno se odjavite i ponovo prijavite.</span><span class="sxs-lookup"><span data-stu-id="1c154-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="1c154-113">Ako se problem ponavlja, otvorite karticu podrške i podiћete ovo kao problem.</span><span class="sxs-lookup"><span data-stu-id="1c154-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="1c154-114">Ako koristite ulogu administratora Exchange servera da biste pristupili centru za bezbednost i usaglašenost, pogledajte sledeći korake.</span><span class="sxs-lookup"><span data-stu-id="1c154-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="1c154-115">Ako aktivirate ulogu da biste pristupili centru za bezbednost i usaglašenost ili ako aktivirate ulogu SharePoint administratora, nailazite na odlaganje aktiviranja od nekoliko minuta do nekoliko časova.</span><span class="sxs-lookup"><span data-stu-id="1c154-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="1c154-116">Ovo je poznati problem i aktivno radimo sa tim timovima da rešimo ovaj problem što je pre moguće.</span><span class="sxs-lookup"><span data-stu-id="1c154-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="1c154-117">Za više informacija pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="1c154-117">For more information, see:</span></span>

- [<span data-ttu-id="1c154-118">Aktiviranje moje Azure OGLASE uloge u PIM</span><span class="sxs-lookup"><span data-stu-id="1c154-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="1c154-119">Aktiviranje moje usluge Azure resursa u PIM</span><span class="sxs-lookup"><span data-stu-id="1c154-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="1c154-120">**Dozvole se ne uklanjaju nakon deaktiviranja uloge ili ističe aktivacija uloge**</span><span class="sxs-lookup"><span data-stu-id="1c154-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="1c154-121">Kada deaktivirate ulogu u usluzi Azure za upravljanje identitetom ili kada istekne period aktivacije uloge, možda će biti kašnjenje gde i dalje imate pristup.</span><span class="sxs-lookup"><span data-stu-id="1c154-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="1c154-122">Ako je vaša deaktivacija odložena, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="1c154-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="1c154-123">Ako deaktivirate ulogu administratora Exchange servera ili istekne period aktivacije uloge, a primetite značajno odlaganje pre nego što se dozvole uklone, otvorite ulaznicu za podršku i obratite se tehničar za podršku da vam pomogne da uradite kaznu sa ekipom za upravljanje pristupom za ovaj problem.</span><span class="sxs-lookup"><span data-stu-id="1c154-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="1c154-124">Ako je period aktivacije istekao, ali i dalje imate otvorenu sesiju pregledača, zatvorite pregledač.</span><span class="sxs-lookup"><span data-stu-id="1c154-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="1c154-125">Možete nastaviti da koristite ulogu dok ne zatvorite tu sesiju.</span><span class="sxs-lookup"><span data-stu-id="1c154-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="1c154-126">Ovo je poznati problem i tražimo potencijalnu popravku da bismo aktivnu opozvali svaku sesiju kada aktivacija istekne.</span><span class="sxs-lookup"><span data-stu-id="1c154-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="1c154-127">Ako je kašnjenje drugačiji od ova dva scenarija, otvorite ulaznicu za podršku.</span><span class="sxs-lookup"><span data-stu-id="1c154-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
