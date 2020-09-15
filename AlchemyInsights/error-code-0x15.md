---
title: Kôd greške 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako dobijate grešku prilikom aktiviranja sistema Office 2013 na udaljenom radnom računaru (RDS), razmotrite omogućavanje ADALA uređivanjem registratora.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709201"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="8429b-103">Greška tokom aktivacije sistema Office 2013 za usluge udaljene radne površine</span><span class="sxs-lookup"><span data-stu-id="8429b-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="8429b-104">Ako dobijate grešku prilikom aktiviranja sistema Office 2013 na udaljenom radnom računaru (RDS), razmotrite omogućavanje ADALA uređivanjem registratora.</span><span class="sxs-lookup"><span data-stu-id="8429b-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="8429b-105">**Ključ registratora**</span><span class="sxs-lookup"><span data-stu-id="8429b-105">**Registry key**</span></span>|<span data-ttu-id="8429b-106">**Zatim**</span><span class="sxs-lookup"><span data-stu-id="8429b-106">**Type**</span></span>|<span data-ttu-id="8429b-107">**Cenimo**</span><span class="sxs-lookup"><span data-stu-id="8429b-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8429b-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="8429b-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="8429b-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="8429b-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="8429b-110">120</span><span class="sxs-lookup"><span data-stu-id="8429b-110">1</span></span>  <br/> |

<span data-ttu-id="8429b-111">Više informacija potražite u članku [Omogućavanje moderne potvrde identiteta za Office 2013 na Windows uređajima](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="8429b-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="8429b-112">ADALA je podrazumevano omogućena u Microsoft 365 aplikacijama za preduzeća i Office 2016.</span><span class="sxs-lookup"><span data-stu-id="8429b-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="8429b-113">Usluge udaljene radne površine (RDS) prethodno su bile imenovane uslugama terminala.</span><span class="sxs-lookup"><span data-stu-id="8429b-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  