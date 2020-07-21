---
title: Brisanje sirotog korisnika sa servera na lokaciji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198589"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="3f883-102">Brisanje sirotog korisnika sa servera na lokaciji</span><span class="sxs-lookup"><span data-stu-id="3f883-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="3f883-103">Da biste uklonili nesirotog korisnika, sledite ove korake:</span><span class="sxs-lookup"><span data-stu-id="3f883-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="3f883-104">Nametni sinhronizaciju direktorijuma prateći uputstva u [čemu je hibridni identitet sa Azure aktivnim direktorijumom?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span><span class="sxs-lookup"><span data-stu-id="3f883-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="3f883-105">Da biste proverili sinhronizaciju direktorijuma, pogledajte [Šta je hibridni identitet sa Azure aktivnim direktorijumom?](https://technet.microsoft.com/library/jj151797.aspx).</span><span class="sxs-lookup"><span data-stu-id="3f883-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="3f883-106">Ako sinhronizacija ispravno funkcioniše, ali se Brisanje objekta aktivnog direktorijuma ne umnožava na Azure oglas, ručno uklonite nepovezani objekat koristeći jedan od sledećih Azure modula aktivnog direktorijuma za Windows PowerShell cmdlet:</span><span class="sxs-lookup"><span data-stu-id="3f883-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="3f883-107">Ukloni-Msolkontakt</span><span class="sxs-lookup"><span data-stu-id="3f883-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="3f883-108">Ukloni-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="3f883-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="3f883-109">Ukloni-MsolUser</span><span class="sxs-lookup"><span data-stu-id="3f883-109">Remove-MsolUser</span></span>

    <span data-ttu-id="3f883-110">Na primer, da biste uklonili nedodeljena ID korisnika john.smith@contoso.com, originalno kreiran pomoću fascikle "sinhronizacija direktorijuma", pokrenite cmdpusti:</span><span class="sxs-lookup"><span data-stu-id="3f883-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="3f883-111">Uklanjanje-MsolUser – korisnički Principalname John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="3f883-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>