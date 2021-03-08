---
title: Evidencija lozinki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527180"
---
# <a name="password-logs"></a><span data-ttu-id="401d3-102">Evidencija lozinki</span><span class="sxs-lookup"><span data-stu-id="401d3-102">Password logs</span></span>

<span data-ttu-id="401d3-103">**Imam problema sa pristupanjem evidenciji nadzora za poništavanje lozinke**</span><span class="sxs-lookup"><span data-stu-id="401d3-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="401d3-104">Da biste rešili probleme u vezi sa pristupom za pristup evidenciji nadzora, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="401d3-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="401d3-105">Obezbedite da imate ovlašćenje za prikaz evidencija nadzora.</span><span class="sxs-lookup"><span data-stu-id="401d3-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="401d3-106">Odobrene su samo sledeće uloge:</span><span class="sxs-lookup"><span data-stu-id="401d3-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="401d3-107">Globalni administrator</span><span class="sxs-lookup"><span data-stu-id="401d3-107">Global administrator</span></span>
 - <span data-ttu-id="401d3-108">Administrator bezbednosti</span><span class="sxs-lookup"><span data-stu-id="401d3-108">Security administrator</span></span>
 - <span data-ttu-id="401d3-109">Čitač bezbednosti</span><span class="sxs-lookup"><span data-stu-id="401d3-109">Security reader</span></span>

<span data-ttu-id="401d3-110">**Želim da vidim sve događaje nadgledanja poništene iz vremena koje sam prvobitno rasporedila**</span><span class="sxs-lookup"><span data-stu-id="401d3-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="401d3-111">Do 120.000 resetovanja lozinki/prijava se skladište u izveštajima prethodnih 30 dana.</span><span class="sxs-lookup"><span data-stu-id="401d3-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="401d3-112">Ovo ograničenje se odnosi na UI kada preuzmete CSV.</span><span class="sxs-lookup"><span data-stu-id="401d3-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="401d3-113">1.000.000 događaji su dostupni kroz PowerShell.</span><span class="sxs-lookup"><span data-stu-id="401d3-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="401d3-114">Dodatne informacije potražite u članku dolenavedene veze:</span><span class="sxs-lookup"><span data-stu-id="401d3-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="401d3-115">Samouslužni događaji poništavaju događaje iz Azure AD izveštaja i API događaja</span><span class="sxs-lookup"><span data-stu-id="401d3-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="401d3-116">Kako da brzo preuzmete događaje registracije lozinki pomoću PowerShell</span><span class="sxs-lookup"><span data-stu-id="401d3-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="401d3-117">**Želim da razumem više o mogućnostima izveštavanja o poništavanju lozinke**</span><span class="sxs-lookup"><span data-stu-id="401d3-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="401d3-118">Potvrdite ko se registruje za ili uspostavlja početnu vrednost lozinki pomoću usluge Azure AD password poništi evidentiranja nadzora na Azure sajtu u okviru **korisnici i grupe**.</span><span class="sxs-lookup"><span data-stu-id="401d3-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="401d3-119">Više informacija potražite u sledećim vezama:</span><span class="sxs-lookup"><span data-stu-id="401d3-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="401d3-120">Pregled izveštaja o poništavanju lozinke</span><span class="sxs-lookup"><span data-stu-id="401d3-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="401d3-121">Kako se prikazuju izveštaji o poništavanju lozinke na Azure portalu</span><span class="sxs-lookup"><span data-stu-id="401d3-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="401d3-122">Samouslužni događaji poništavaju događaje iz Azure AD izveštaja i API događaja</span><span class="sxs-lookup"><span data-stu-id="401d3-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="401d3-123">Kako da brzo preuzmete događaje registracije lozinki pomoću PowerShell</span><span class="sxs-lookup"><span data-stu-id="401d3-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


