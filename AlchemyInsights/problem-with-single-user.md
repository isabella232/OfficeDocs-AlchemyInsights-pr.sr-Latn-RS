---
title: Problem sa jednim korisnikom
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430205"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="c59f3-102">Problem sa jednim korisnikom</span><span class="sxs-lookup"><span data-stu-id="c59f3-102">Problem with single user</span></span>

- <span data-ttu-id="c59f3-103">Korisnik možda nije dodeljen zato što usluga još uvek nije imala priliku da proceni korisnika.</span><span class="sxs-lookup"><span data-stu-id="c59f3-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="c59f3-104">Pregledajte smernice za koliko traje obezbeđivanje, kao i traka toka vremena, na stranici za konfigurisanje obezbeđivanja.</span><span class="sxs-lookup"><span data-stu-id="c59f3-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="c59f3-105">Ako se čvrsto stanje navedeno u odeljku dodatni detalji nalazi pre datuma kada je korisnik kreiran/ažuriran/izbrisan, to znači da još uvek nismo procenili korisnika.</span><span class="sxs-lookup"><span data-stu-id="c59f3-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="c59f3-106">U ovom scenariju, najbolje je da sačekate da se završi usluga obezbeđivanje.</span><span class="sxs-lookup"><span data-stu-id="c59f3-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="c59f3-107">Imajte u vidu da je naša usluga samo svesna promena u korisniku u izvornom sistemu (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="c59f3-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="c59f3-108">Mora da postoji važeća promena u izvornom sistemu za Azure AD da biste otkrili promenu i doišli u aktivni direktorijum.</span><span class="sxs-lookup"><span data-stu-id="c59f3-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="c59f3-109">Polje za obezbeđivanje je procenilo korisnika i utvrđeno je da ne bi trebalo da bude dodeljen:</span><span class="sxs-lookup"><span data-stu-id="c59f3-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="c59f3-110">Ako ste konfigurisali filter zasnovan na atributu, uverite se da korisnik ispunjava kriterijume koje ste naveli.</span><span class="sxs-lookup"><span data-stu-id="c59f3-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="c59f3-111">Ako korisnici već postoje u ciljnom sistemu i stanju korisnika u odnosu na izvor i ciljnu verziju, nećemo preduzimati nikakvu dalju radnju.</span><span class="sxs-lookup"><span data-stu-id="c59f3-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="c59f3-112">Usluga obezbeđivanja pokušava da dodeli korisnika i nije uspela.</span><span class="sxs-lookup"><span data-stu-id="c59f3-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="c59f3-113">Za ove scenarije Pregledajte karticu Rešavanje problema i preporuke za evidentiranje stavki:</span><span class="sxs-lookup"><span data-stu-id="c59f3-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="c59f3-114">Zahtevani atribut na korisniku možda nedostaje u lokalnom programu Active Directory ili Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c59f3-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c59f3-115">Na primer, korisnički Principalname ili pravila za generaciju imena ne generišu odgovarajuću vrednost.</span><span class="sxs-lookup"><span data-stu-id="c59f3-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="c59f3-116">Podudarni atribut (obično je zaposlenom) ne rešava jedinstvenog korisnika u lokalnom aktivnom direktorijumu ili Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c59f3-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c59f3-117">Na primer, postoje dva korisnika sa istim zaposlenim ID-om u REKLAMI i usluga vraća kôd greške koji označava duplirane odredišne stavke za istu izvornu stavku.</span><span class="sxs-lookup"><span data-stu-id="c59f3-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="c59f3-118">Da biste pregledali evidentiranje za jednog korisnika i grupe, pogledajte [članak Pregledanje evidencija resursa za problem sa određenim korisnikom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="c59f3-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
