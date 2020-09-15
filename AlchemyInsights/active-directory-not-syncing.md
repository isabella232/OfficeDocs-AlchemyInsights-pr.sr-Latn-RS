---
title: Aktivni direktorijum se ne sinhronizuje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697643"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="ce51e-102">Aktivni direktorijum se ne sinhronizuje</span><span class="sxs-lookup"><span data-stu-id="ce51e-102">Active Directory not syncing</span></span>

<span data-ttu-id="ce51e-103">Ako primate greške sinhronizacije, kao što je "nije došlo do nedavne sinhronizacije" ili primetite da status sinhronizacije direktorijuma na Office administratorskim portisima piše, "poslednji put sinhronizovan pre više od 3 dana", može biti da AADConnect ima neispravne postavke ili nije imala dovoljne dozvole za sinhronizaciju.</span><span class="sxs-lookup"><span data-stu-id="ce51e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="ce51e-104">Ponovna instalacija AADConnect pomoću postavki Ekspresna može brzo rešiti problem:</span><span class="sxs-lookup"><span data-stu-id="ce51e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="ce51e-105">[Preuzmite najnoviju verziju programa AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="ce51e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="ce51e-106">[Izvršite uputstva za ekspresnu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="ce51e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="ce51e-107">Više informacija o AADConnect nalozima usluge potražite u članku [Azure AD Connect: nalozi i dozvole](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="ce51e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
