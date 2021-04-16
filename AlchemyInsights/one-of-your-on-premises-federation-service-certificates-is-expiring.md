---
title: Jedan od certifikata za uslugu za probnu upotrebu usluge za ubuduće iskoči
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810066"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="7d6bb-102">Jedan od certifikata za uslugu za probnu upotrebu usluge za ubuduće iskoči</span><span class="sxs-lookup"><span data-stu-id="7d6bb-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="7d6bb-103">Da biste rešili ovaj problem, pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="7d6bb-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="7d6bb-104">Instalirajte modul Microsoft Azure Active Directory za Windows PowerShell na računaru (ako modul nije već instaliran).</span><span class="sxs-lookup"><span data-stu-id="7d6bb-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="7d6bb-105">Da biste to uradio, idite [na Azure Active Directory PowerShell za Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="7d6bb-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="7d6bb-106">Pratite korake u odeljku "1. slučaj: Istekao je certifikat za potpisivanje AD FS tokena" u odeljku "Došlo je do problema prilikom pristupa sajtu" iz usluge AD FS kada se federan korisnik prijavi u [Microsoft 365, Azure ili Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="7d6bb-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="7d6bb-107">Pratite korake u članku Ažuriranje ili popravljanje postavki federanog domena u uslugama [Microsoft 365, Azure ili Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)</span><span class="sxs-lookup"><span data-stu-id="7d6bb-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="7d6bb-108">Više informacija o obnavljanju certifikata za federation potražite u temi Obnavljanje certifikata za [O365 i Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="7d6bb-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

