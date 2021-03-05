---
title: Problem sa atributom i skping filtriranjem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482920"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="c3252-102">Problem sa atributom i skping filtriranjem</span><span class="sxs-lookup"><span data-stu-id="c3252-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="c3252-103">**Problem sa neusaglašenim UPN vrednostima**</span><span class="sxs-lookup"><span data-stu-id="c3252-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="c3252-104">Radni dan za obezbeđivanje korisničkog radnog dana za OGLAŠAVANJE u AD User prikazuje poruku o grešci **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="c3252-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="c3252-105">Operacija nije uspela zato što UPN vrednost obezbeđena za sabiranje/modifikacija nije jedinstvena Šumska suma.</span><span class="sxs-lookup"><span data-stu-id="c3252-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="c3252-106">Detalji greške: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="c3252-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="c3252-107">Vrednost " **Userprincipalname** " koji pokušava da podesi prilikom pravljenja oglasa korisničkog naloga već postoji u DOMENU Target a.d..</span><span class="sxs-lookup"><span data-stu-id="c3252-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="c3252-108">To implicira da (1) korisnik već postoji i da funkcija podudaranja sa ID-om nije uspela za korisnika ili (2) pravilo generacije UPN je Generisano neusaglašenu vrednost.</span><span class="sxs-lookup"><span data-stu-id="c3252-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="c3252-109">Evo koraka predloga rezolucije:</span><span class="sxs-lookup"><span data-stu-id="c3252-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="c3252-110">Ako korisnik već postoji i kada se podudarna identifikacija identiteta nije uspela, povežite se sa radnim danom nalogom na Active Directory nalog, a zatim potvrdite izbor u polju za proveru</span><span class="sxs-lookup"><span data-stu-id="c3252-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="c3252-111">Ako nemaju podudaranje, to je problem sa podacima koji treba da se popravi.</span><span class="sxs-lookup"><span data-stu-id="c3252-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="c3252-112">Na primer, ako je ID zaposlenog u toku posla 001052 i u programu AD je 1052, polje za obezbeđivanje može da se poveže sa dva naloga i pokušaće da kreira korisnika koji već postoji.</span><span class="sxs-lookup"><span data-stu-id="c3252-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="c3252-113">Rešenje u ovom slučaju je da promenite vrednost **Zaposleneid** u reklami da biste uključene glavne nule da biste je napravili 001052.</span><span class="sxs-lookup"><span data-stu-id="c3252-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="c3252-114">Ako izrazi koji generišu UPN ne generišu jedinstvenu vrednost, razmotrite korišćenje funkcije dedupliranje funkcija **Seledequevalue** prilikom svakog kreiranja jedinstvene vrednosti.</span><span class="sxs-lookup"><span data-stu-id="c3252-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="c3252-115">**Radni dan za obezbeđivanje oglašavanja korisnika ne podešava vrednost atributa Menadžera za adninalog korisnika**</span><span class="sxs-lookup"><span data-stu-id="c3252-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="c3252-116">Radni dan za obezbeđivanje oglasa korisnika ne postavlja vrednost atributa **Menadžera** za AD User naloge.</span><span class="sxs-lookup"><span data-stu-id="c3252-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="c3252-117">Postoje dva moguća scenarija kada se ovo ponašanje vidi:</span><span class="sxs-lookup"><span data-stu-id="c3252-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="c3252-118">Menadžer u radnom mestu ne može da se razreši na odgovarajući korisnički nalog za AD zato što menadžer nije u opsegu.</span><span class="sxs-lookup"><span data-stu-id="c3252-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="c3252-119">U okviru **višestruki** domeni scenariji, menadžer u toku posla nije prisutan u istom domenu kao korisnik.</span><span class="sxs-lookup"><span data-stu-id="c3252-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="c3252-120">Isprobajte ove korake da biste rešili problem:</span><span class="sxs-lookup"><span data-stu-id="c3252-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="c3252-121">Ako ste definisali skping filtere, prvo proverite da li se menadžer nalazi u opsegu i da li ispunjava klauzulu.</span><span class="sxs-lookup"><span data-stu-id="c3252-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="c3252-122">Ako Menadžer ne zadovoljava filter za skping, promenite filter tako da je i menadžer u okviru operacije obezbeđivanje.</span><span class="sxs-lookup"><span data-stu-id="c3252-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="c3252-123">Ako imate više oglasa, onda konektor ima poznato ograničenje nesposobnosti da rešava reference menadžera unakrsnog domena.</span><span class="sxs-lookup"><span data-stu-id="c3252-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="c3252-124">Za više detalja o konfigurisanju radnog vremena za automatizovano obezbeđivanje pogledajte [članak uputstvo: konfigurisanje radnog dana za automatsko obezbeđivanje korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="c3252-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













