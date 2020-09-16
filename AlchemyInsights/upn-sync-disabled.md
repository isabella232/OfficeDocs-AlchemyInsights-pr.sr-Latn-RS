---
title: UPN sinhronizacija je omogućena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749528"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="b6a43-102">UPN sinhronizacija je omogućena</span><span class="sxs-lookup"><span data-stu-id="b6a43-102">UPN sync disabled</span></span>

<span data-ttu-id="b6a43-103">Ako ste započeli sinhronizaciju sa Azure AD pre 30.2016, uradite sledeće Azure AD PowerShell cmdlet usluge da biste omogućili UPN Meki podudaranje samo za vašu organizaciju:</span><span class="sxs-lookup"><span data-stu-id="b6a43-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="b6a43-104">**Funkcija for-Msoldirsyncfunkcije-Enablesoftprovoonupn-omogućavanje $True**</span><span class="sxs-lookup"><span data-stu-id="b6a43-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="b6a43-105">UPN meka podudaranje automatski se uključuje za organizacije koje su počele da se sinhronizuju sa uslugom Azure AD ili posle 2016 30.</span><span class="sxs-lookup"><span data-stu-id="b6a43-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="b6a43-106">Da biste saznali više o omogućavanju mekog podudaranja na UPN i drugim funkcijama sinhronizacije, pogledajte članak [funkcije Azure AD Connect sinhronizacija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="b6a43-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

