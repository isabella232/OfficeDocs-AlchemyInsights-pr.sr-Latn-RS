---
title: Smernice grupe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256786"
---
# <a name="group-policy"></a><span data-ttu-id="93529-102">Smernice grupe</span><span class="sxs-lookup"><span data-stu-id="93529-102">Group policy</span></span>

<span data-ttu-id="93529-103">Postavke za korisničke i kompjuterske objekte u uslugama usluge Azure Active Directory (Azure AD DS) se često upravljaju korišćenjem objekata smernica grupe (GPOs).</span><span class="sxs-lookup"><span data-stu-id="93529-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="93529-104">Azure reklame uključuju ugrađene GPOs za korisnike AADDC korisnika i AADDC kompjutere.</span><span class="sxs-lookup"><span data-stu-id="93529-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="93529-105">Ove ugrađene GPOs možete prilagoditi da biste podesili smernice grupe po potrebi za okruženje.</span><span class="sxs-lookup"><span data-stu-id="93529-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="93529-106">Članovi grupe Azure AD DC Administratori imaju privilegije administracije grupnih smernica u domenu Azure AD DS i mogu da kreiraju prilagođene GPOs i organizacione jedinice (use).</span><span class="sxs-lookup"><span data-stu-id="93529-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="93529-107">Više informacija o tome koje su smernice grupe i kako ona funkcioniše potražite u članku [Pregled smernica grupe](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="93529-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="93529-108">U hibridnim okruženju, smernice grupe podešene u lokalnom programu za okruženje nisu sinhronizovane sa uslugom Azure ADS.</span><span class="sxs-lookup"><span data-stu-id="93529-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="93529-109">Da biste definisali postavke konfiguracije za korisnike ili računare u usluzi Azure ADS, uredite jedan od podrazumevanih GPOs ili Kreirajte prilagođeni GPO.</span><span class="sxs-lookup"><span data-stu-id="93529-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="93529-110">Ovaj članak [upravlja smernicama grupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) pokazuje kako da instalirate alatke za upravljanje smernicama grupe, kako ton uređuje ugrađene GPOs i kako da kreirate prilagođene GPOs.</span><span class="sxs-lookup"><span data-stu-id="93529-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



