---
title: Sinhronizacija lozinki za uslugu Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177623"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="69463-102">Sinhronizacija lozinki za uslugu Domain</span><span class="sxs-lookup"><span data-stu-id="69463-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="69463-103">**Ako vam je instanca "Azure AD DS" upitna da omogućite sinhronizaciju hash sinhronizacije lozinki**</span><span class="sxs-lookup"><span data-stu-id="69463-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="69463-104">Nailazite na scenario u kojem koristite hibridno okruženje sa korisnicima sinhronizuju iz lokalnog Azure Active Directory Services domena (AD DS) okruženja.</span><span class="sxs-lookup"><span data-stu-id="69463-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="69463-105">Ovaj scenario se susreće bez obzira na to da li ste sinhronizuju lozinke hash usluge u lokalnim OGLADIMA sa vašim Azure AD zakupcem.</span><span class="sxs-lookup"><span data-stu-id="69463-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="69463-106">**Uzrok**</span><span class="sxs-lookup"><span data-stu-id="69463-106">**Cause**</span></span>

<span data-ttu-id="69463-107">To se dešava zato što Azure AD Connect po podrazumevanoj vrednosti ne sinhronizuje zastareli novi tehnološki LAN Manager (NTLM) i Kerberos hash lozinke koji su neophodni za Azure ADS.</span><span class="sxs-lookup"><span data-stu-id="69463-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="69463-108">**Privremeno rešenje**</span><span class="sxs-lookup"><span data-stu-id="69463-108">**Workaround**</span></span> 

<span data-ttu-id="69463-109">Trebalo bi da konfigurišete Azure AD Connect da biste sinhronizovali te lozinke koje su potrebne za NTLM i Kerberos potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="69463-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="69463-110">Kada se konfiguriše Azure AD Connect, pravljenje lokalnog naloga ili događaj promene lozinki takođe sinhronizuje hash nasleđene lozinke u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="69463-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="69463-111">Pogledajte [ovde](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) za više informacija o tome i za uputstva o tome kako se omogućava sinhronizacija lozinki u usluzi AZURE AD DS hibridna okruženja.</span><span class="sxs-lookup"><span data-stu-id="69463-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>