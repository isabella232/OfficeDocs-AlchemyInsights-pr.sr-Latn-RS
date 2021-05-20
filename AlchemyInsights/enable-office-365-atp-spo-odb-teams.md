---
title: Omogućite Office 365 ATP za SharePoint, OneDrive, i Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543942"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="508fb-102">Omogućite Microsoft zaštitnik za Office 365 za SharePoint na mreži, OneDrive, kao i za Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="508fb-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="508fb-103">Idite na https://protection.office.com i prijavite se.</span><span class="sxs-lookup"><span data-stu-id="508fb-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="508fb-104">Odaberite **stavku**  >  **Smernice za**  >  **upravljanje pretnjama Sef prilozima.**</span><span class="sxs-lookup"><span data-stu-id="508fb-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="508fb-105">Izaberite **stavku Uključi zaštitnik za Office 365 za SharePoint, OneDrive i Microsoft Teams**, a zatim kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="508fb-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="508fb-106">(Preporučeno) Kao globalni administrator ili administrator SharePoint na mreži, pokrenite cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) sa **disallowInfectedFileDownload** parametar postavljenim na *vrednost true.*</span><span class="sxs-lookup"><span data-stu-id="508fb-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="508fb-107">(Preporučeno) [Podesite obaveštenja za](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) otkrivene datoteke.</span><span class="sxs-lookup"><span data-stu-id="508fb-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="508fb-108">Microsoft zaštitnik za Office 365 skenira svaku datoteku u uslugama SharePoint Online, OneDrive ili Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="508fb-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="508fb-109">Datoteke se skeniraju as sinhrono, kroz proces koji koristi događaje deljenja i aktivnosti gosta, zajedno sa pametnim heuristicama i signalima pretnji za identifikovanje zlonamernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="508fb-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="508fb-110">Pogledajte [članak Microsoft zaštitnik za Office 365 za SharePoint, OneDrive i Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="508fb-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>