---
title: Rešavanje problema sa OneDrive performansama
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757899"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="a8ec5-102">Rešavanje problema sa OneDrive performansama</span><span class="sxs-lookup"><span data-stu-id="a8ec5-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="a8ec5-103">Ako imate sporu od očekivane sinhronizovane probleme sa performansama u usluzi OneDrive:</span><span class="sxs-lookup"><span data-stu-id="a8ec5-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="a8ec5-104">Potvrdite da ne postoje poznati problemi pomoću [kontrolne table zdravstvenog usluge](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a8ec5-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="a8ec5-105">[Omogućite datoteke na zahtev](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) tako da možete da pristupite svim datotekama u usluzi OneDrive bez potrebe da preuzmete sve njih i koristite prostor za skladištenje na uređaju.</span><span class="sxs-lookup"><span data-stu-id="a8ec5-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="a8ec5-106">[Pregledajte najbolje prakse](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) za planiranje mreže i performanse.</span><span class="sxs-lookup"><span data-stu-id="a8ec5-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="a8ec5-107">[Uvećajte otpremanje i brzinu preuzimanja](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), naročito ako prvi put sinhronizujete uređaj.</span><span class="sxs-lookup"><span data-stu-id="a8ec5-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="a8ec5-108">Ako sinhronizujete biblioteku sa više od 100.000 stavki, sinhronizacija usluge OneDrive može biti dugo zaglavljena, a status prikazuje obradu 0KB od xMB. "</span><span class="sxs-lookup"><span data-stu-id="a8ec5-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="a8ec5-109">[Saznajte više o sinhronizovanju više od 100.000 datoteka](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , kao i o [300.000 ograničenju usluge OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="a8ec5-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="a8ec5-110">Kada korisnik premaši ograničenja upotrebe, SharePoint online radi sa svim dalje zahtjevima sa tog korisničkog naloga na kratak period.</span><span class="sxs-lookup"><span data-stu-id="a8ec5-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="a8ec5-111">Sve korisničke radnje se potiskuju dok je regulator gasa na snazi.</span><span class="sxs-lookup"><span data-stu-id="a8ec5-111">All user actions are throttled while the throttle is in effect.</span></span>
