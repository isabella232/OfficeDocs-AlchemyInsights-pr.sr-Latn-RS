---
title: Radnje programa Windows Defender u Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1282"
- "6700008"
ms.openlocfilehash: 61a2411ce7c4578ecf2c32943c6a21edbf63eeee
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440444"
---
# <a name="windows-defender-actions-in-intune"></a><span data-ttu-id="f9c3a-102">Radnje programa Windows Defender u Intune</span><span class="sxs-lookup"><span data-stu-id="f9c3a-102">Windows Defender actions in Intune</span></span>

<span data-ttu-id="f9c3a-103">Intune može da se koristi za pokretanje ažuriranja na zahtev za skeniranje i potpis virusa za Windows Defender na pojedinačnim uređajima.</span><span class="sxs-lookup"><span data-stu-id="f9c3a-103">Intune can be used to trigger an on-demand scan and virus signature update for Windows Defender on individual devices.</span></span>

<span data-ttu-id="f9c3a-104">Kada je udaljena radnja uspešno pokrenuta, aktivnost se odražava na evidenciju događaja programa Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="f9c3a-104">After a remote action is successfully triggered the activity is reflected in the Windows Defender event log.</span></span>

<span data-ttu-id="f9c3a-105">Windows smernice za zaštitu krajnje tačke omogućavaju da se dodatne postavke za funkcije programa Windows Defender kreiraju u usluzi Intune i primeni na skupove uređaja.</span><span class="sxs-lookup"><span data-stu-id="f9c3a-105">Windows Endpoint Protection policy allows additional settings for Windows Defender features to be created in Intune and applied to sets of devices.</span></span>

<span data-ttu-id="f9c3a-106">Više detalja o aktiviranju radnji programa Windows Defender potražite [u članku Konfigurisanje i izvršavanje zahteva za Microsoft Defender antivirusnim skenima](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="f9c3a-106">For more details on triggering Windows Defender actions, see [Configure and run on-demand Microsoft Defender Antivirus scans](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/run-scan-windows-defender-antivirus).</span></span>