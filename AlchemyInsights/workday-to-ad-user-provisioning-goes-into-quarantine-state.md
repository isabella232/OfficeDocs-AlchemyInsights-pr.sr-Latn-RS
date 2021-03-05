---
title: Radni dan za obezbeđivanje oglasa korisnika ide u stanje karantina
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482902"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="76eaf-102">Radni dan za obezbeđivanje oglasa korisnika ide u stanje karantina</span><span class="sxs-lookup"><span data-stu-id="76eaf-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="76eaf-103">**Radni dan za obezbeđivanje oglasa korisnika prelazi u stanje karantina i nijedan korisnik se ne kreira u OGLASU**</span><span class="sxs-lookup"><span data-stu-id="76eaf-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="76eaf-104">Radni dan za obezbeđivanje OGLAŠAVANJA za korisnika je otišao u stanje karantina, a evidentiranje nadzora prikazuje događaje izvoza pomoću greške sa porukom o grešci **: Operationser. Nije podešena nijedna superiorna referenca za uslugu direktorijuma. Usluga direktorijuma stoga ne može da izda referente objekte izvan ove šume**.</span><span class="sxs-lookup"><span data-stu-id="76eaf-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="76eaf-105">Do ove greške obično dolazi ako kontejner Active Directory nije ispravno podešen ili ako postoje problemi sa mapiranjem izraza koje se koristi za **Parent.**</span><span class="sxs-lookup"><span data-stu-id="76eaf-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="76eaf-106">Potvrdite izbor u podrazumevanom dijalogu za **novi korisnici** parametra za Tipos.</span><span class="sxs-lookup"><span data-stu-id="76eaf-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="76eaf-107">Uverite se da navedeno koje već postoji u vašem OGLASU.</span><span class="sxs-lookup"><span data-stu-id="76eaf-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="76eaf-108">Ako koristite **Parent, Izhedime** u mapiranju atributa, uverite se da se uvek izračunava na poznat kontejner unutar domena oglasa.</span><span class="sxs-lookup"><span data-stu-id="76eaf-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="76eaf-109">Pogledajte događaj izvoza u evidenciji nadzora da biste videli generisane vrednosti.</span><span class="sxs-lookup"><span data-stu-id="76eaf-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="76eaf-110">Za više detalja o konfigurisanju radnog vremena za automatizovano obezbeđivanje pogledajte [članak uputstvo: konfigurisanje radnog dana za automatsko obezbeđivanje korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="76eaf-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

