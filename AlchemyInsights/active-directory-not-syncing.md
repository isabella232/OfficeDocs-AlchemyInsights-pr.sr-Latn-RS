---
title: Active Directory se ne sinhronizuje
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930989"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="7ec26-102">Active Directory se ne sinhronizuje</span><span class="sxs-lookup"><span data-stu-id="7ec26-102">Active Directory not syncing</span></span>

<span data-ttu-id="7ec26-103">Ako primate greške prilikom sinhronizacije, na primer "nema nedavne sinhronizacije" ili primetite da status sinhronizacije direktorijuma na Kancelarija portalu za adminitre kaže "Poslednji put sinhronizovano pre više od 3 dana", moguće je da AADConnect ima neispravne postavke ili nedovoljne dozvole za izvršavanje sinhronizacije.</span><span class="sxs-lookup"><span data-stu-id="7ec26-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="7ec26-104">Poništavanje usluge AADConnect pomoću ekspresnih postavki može brzo da reši problem:</span><span class="sxs-lookup"><span data-stu-id="7ec26-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="7ec26-105">[Preuzmite najnoviju verziju AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="7ec26-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="7ec26-106">[Pratite uputstva za ekspresnu instalaciju](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="7ec26-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="7ec26-107">Azure AD Connect mora da se instalira na Windows serveru 2012 ili novijoj verziji.</span><span class="sxs-lookup"><span data-stu-id="7ec26-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="7ec26-108">Ovaj server mora da bude pridružen domenu i može da bude kontroler domena ili server član.</span><span class="sxs-lookup"><span data-stu-id="7ec26-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="7ec26-109">Kompletnu listu Azure AD Povezivanje zahteve i preduslove, pregledajte preduslove za [Azure AD Povezivanje.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="7ec26-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="7ec26-110">Više informacija o AADConnect nalozima usluge potražite u temi [Azure AD Povezivanje:](/azure/active-directory/hybrid/reference-connect-accounts-permissions)Nalozi i dozvole.</span><span class="sxs-lookup"><span data-stu-id="7ec26-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
