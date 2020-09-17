---
title: 932 nadogradnja AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806053"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="6c1a2-102">Nadogradnja Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="6c1a2-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="6c1a2-103">Automatski Nadogradnja je podrazumevano omogućena za Azure AD Connect što pomaže da se osigura da pokrećete najnoviju verziju.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="6c1a2-104">Da biste verifikovali postavke automatske nadogradnje, koristite cmdlet karticu " **Nabavite-Adsynkotouprazred** " u usluzi AZURE AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="6c1a2-105">Cmdlet će vratiti jednu od sledećih vrednosti:</span><span class="sxs-lookup"><span data-stu-id="6c1a2-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="6c1a2-106">**Omogućeno**: automatsko Nadogradnja je omogućena.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="6c1a2-107">**Onemogući**: automatsko Nadogradnja je onemogućiti.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="6c1a2-108">**Obustavljeno**: sistem više ne može da prima automatska nadogradnje.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="6c1a2-109">Ne možete da konfigurišete ovu vrednost; Podešava ga sistem.</span><span class="sxs-lookup"><span data-stu-id="6c1a2-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="6c1a2-110">Više informacija potražite u članku [Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="6c1a2-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="6c1a2-111">Da biste preuzeli najnoviju verziju usluge Azure AD Connect, idite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="6c1a2-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
