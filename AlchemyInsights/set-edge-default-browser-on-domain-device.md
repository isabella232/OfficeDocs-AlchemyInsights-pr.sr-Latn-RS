---
title: Podešavanje pregledača Microsoft Edge kao podrazumevanog pregledača na uređaju pridruženog domenu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491880"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="87602-102">Podešavanje pregledača Microsoft Edge kao podrazumevanog pregledača na uređaju pridruženog domenu</span><span class="sxs-lookup"><span data-stu-id="87602-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="87602-103">Postavite Microsoft Edge kao podrazumevani pregledač:</span><span class="sxs-lookup"><span data-stu-id="87602-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="87602-104">[Kreirajte podrazumevanu datoteku konfiguracije povezanosti](https://go.microsoft.com/fwlink/?linkid=2132437) i uskladištite je lokalno ili na mrežnom resursu.</span><span class="sxs-lookup"><span data-stu-id="87602-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="87602-105">Otvorite uređivač smernica grupe, a zatim idite na stavku **Administrativni**  >  **predlošci** za  >  **konfiguraciju** računara Windows istraživač  >  **datoteka.**</span><span class="sxs-lookup"><span data-stu-id="87602-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="87602-106">Izaberite **stavku Postavljanje podrazumevane datoteke konfiguracije povezanosti**.</span><span class="sxs-lookup"><span data-stu-id="87602-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="87602-107">Izaberite **postavku smernica**, a zatim **izaberite Stavku Omogućeno**.</span><span class="sxs-lookup"><span data-stu-id="87602-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="87602-108">U **okviru** Opcije unesite lokaciju podrazumevane datoteke konfiguracije povezanosti, a zatim kliknite na dugme **U redu.**</span><span class="sxs-lookup"><span data-stu-id="87602-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
