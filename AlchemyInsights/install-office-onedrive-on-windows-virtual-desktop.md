---
title: Instaliranje sistema Office i usluge OneDrive na Windows virtuelnoj radnoj površini
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595841"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="5aefc-102">Instaliranje sistema Office i usluge OneDrive na Windows virtuelnoj radnoj površini</span><span class="sxs-lookup"><span data-stu-id="5aefc-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="5aefc-103">[Priprema i prilagođavanje master VHD slike](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span><span class="sxs-lookup"><span data-stu-id="5aefc-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="5aefc-104">Kreirajte virtuelnu mašinu (VM) ako već nije kreirana.</span><span class="sxs-lookup"><span data-stu-id="5aefc-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="5aefc-105">[Instalirajte Office u režimu aktivacije deljenog računara.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="5aefc-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="5aefc-106">Aktivacija deljenog računara omogućava većem broju korisnika da pristupe office programu.</span><span class="sxs-lookup"><span data-stu-id="5aefc-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="5aefc-107">[Instalirajte OneDrive u režimu po računaru.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="5aefc-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="5aefc-108">Obično se OneDrive instalira po korisniku, ali ovde bi trebalo da se instalira po računaru.</span><span class="sxs-lookup"><span data-stu-id="5aefc-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>