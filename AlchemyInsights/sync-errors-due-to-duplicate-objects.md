---
title: 902 (greške sinhronizacije zbog dupliranih objekata)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708076"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="70b36-102">Greške pri sinhronizaciji zbog dupliranih objekata</span><span class="sxs-lookup"><span data-stu-id="70b36-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="70b36-103">Možete primiti jednu od sledećih poruka o grešci kada se sinhronizacija direktorijuma završi u programu Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="70b36-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="70b36-104">Nije moguće ažurirati ovaj objekat u Microsoft usluzi na mreži zato što sledeći atributi povezani sa ovim objektom imaju vrednosti koji su možda već povezani sa drugim objektom u lokalnom direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="70b36-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="70b36-105">Sinhronizovani objekat sa istom proxy adresom već postoji u usluzi Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="70b36-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="70b36-106">Nije moguće ažurirati ovaj objekat zato što sledeći atributi povezani sa ovim objektom imaju vrednosti koji su možda već povezani sa drugim objektom u lokalnim direktorijima: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="70b36-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="70b36-107">Da biste identifikovali i rešili problem, preuzmite i uradite alatku za rešavanje problema sa [Idfix DirSync](https://github.com/Microsoft/idfix).</span><span class="sxs-lookup"><span data-stu-id="70b36-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="70b36-108">Više informacija potražite u članku [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="70b36-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
