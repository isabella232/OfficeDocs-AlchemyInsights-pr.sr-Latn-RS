---
title: Korišćenje usluge Exchange online PowerShell za omogućavanje DKIM za određeni domen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749729"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="6089f-102">Korišćenje usluge Exchange online PowerShell za omogućavanje DKIM za određeni domen</span><span class="sxs-lookup"><span data-stu-id="6089f-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="6089f-103">Ako ne možete da kreirate DKIM DNS zapise u centru administracije, probajte da koristite Exchange online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6089f-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="6089f-104">Da biste kreirali DKIM DNS zapis pomoću usluge Exchange online PowerShell, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="6089f-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="6089f-105">Otvorite Windows PowerShell kao administrator i uradite sledeće komande u opisanom redosledu:</span><span class="sxs-lookup"><span data-stu-id="6089f-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="6089f-106">Neko.</span><span class="sxs-lookup"><span data-stu-id="6089f-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="6089f-107">-.</span><span class="sxs-lookup"><span data-stu-id="6089f-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="6089f-108">trojku.</span><span class="sxs-lookup"><span data-stu-id="6089f-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="6089f-109">Ako imate problema sa povezivanjem sa uslugom Exchange online PowerShell, pogledajte članak [Povezivanje sa uslugom Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="6089f-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="6089f-110">Kada se povežete sa Exchange online PowerShell, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="6089f-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="6089f-111">Kada se gorenavedenu komanda uspešno izvrši, uradite sledeću komandu da biste prekinuli Exchange online sesiju PowerShell sesije:</span><span class="sxs-lookup"><span data-stu-id="6089f-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



