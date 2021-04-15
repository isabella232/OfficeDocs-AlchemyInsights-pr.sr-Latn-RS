---
title: UPN sinhronizacija je onemogućena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782165"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="def2b-102">UPN sinhronizacija je onemogućena</span><span class="sxs-lookup"><span data-stu-id="def2b-102">UPN sync disabled</span></span>

<span data-ttu-id="def2b-103">Ako ste počeli da sinhronizujete sa uslugom Azure AD pre 30. marta 2016. godine, pokrenite sledeću Azure AD PowerShell cmdlet da biste omogućili UPN uslovno podudaranje samo za organizaciju:</span><span class="sxs-lookup"><span data-stu-id="def2b-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="def2b-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="def2b-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="def2b-105">UPN meko podudaranje automatski je uključeno za organizacije koje su započele sinhronizaciju sa Azure AD uključene ili posle 30. marta 2016.</span><span class="sxs-lookup"><span data-stu-id="def2b-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="def2b-106">Da biste saznali više o omogućavanju mekih podudaranja u UPN-u i drugim funkcijama sinhronizacije, pogledajte [TPG Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)funkcije usluge sinhronizacije.</span><span class="sxs-lookup"><span data-stu-id="def2b-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

