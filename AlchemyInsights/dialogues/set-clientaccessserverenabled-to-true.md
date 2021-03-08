---
title: Podesi ClientAccessServerEnabled na TRUE
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525963"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="936bf-102">Podesi ClientAccessServerEnabled na TRUE</span><span class="sxs-lookup"><span data-stu-id="936bf-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="936bf-103">Ako ne možete da otvorite šifrovanu e-poruku i da vidite prilog **rpmsg** , izvršite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="936bf-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="936bf-104">Povezivanje sa uslugom Exchange online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="936bf-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="936bf-105">Da biste se povezali sa uslugom Exchange online PowerShell, morate da se prijavite pomoću globalnog administratora ili Exchange naloga administracije.</span><span class="sxs-lookup"><span data-stu-id="936bf-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="936bf-106">Neko.</span><span class="sxs-lookup"><span data-stu-id="936bf-106">a.</span></span> <span data-ttu-id="936bf-107">Otvorite Windows PowerShell, a zatim uradite sledeće: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="936bf-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="936bf-108">-.</span><span class="sxs-lookup"><span data-stu-id="936bf-108">b.</span></span> <span data-ttu-id="936bf-109">U dijalogu **zahtev za akreditiva Windows PowerShell** unesite poslovni ili školski nalog i lozinku, c.</span><span class="sxs-lookup"><span data-stu-id="936bf-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="936bf-110">Kliknite na dugme **U redu**.</span><span class="sxs-lookup"><span data-stu-id="936bf-110">Click **OK**.</span></span> 

2. <span data-ttu-id="936bf-111">Uradite sledeće komande da biste kreirali novu sesiju:</span><span class="sxs-lookup"><span data-stu-id="936bf-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="936bf-112">Neko.</span><span class="sxs-lookup"><span data-stu-id="936bf-112">a.</span></span> <span data-ttu-id="936bf-113">Uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="936bf-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="936bf-114">`Get-IRMConfiguration`Komanda "pokrene".</span><span class="sxs-lookup"><span data-stu-id="936bf-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="936bf-115">Potvrdite postavku **Clientaccessserverenabled** .</span><span class="sxs-lookup"><span data-stu-id="936bf-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="936bf-116">Neko.</span><span class="sxs-lookup"><span data-stu-id="936bf-116">a.</span></span> <span data-ttu-id="936bf-117">Ako je postavka **Clientaccessserverenabled** postavljena na **vrednost FALSE**, uradite sledeće cmdlet lokacije: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="936bf-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="936bf-118">Uvek zatvorite sesiju PowerShell sa sledećim komandama: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="936bf-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="936bf-119">Više informacija potražite u članku [Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="936bf-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

