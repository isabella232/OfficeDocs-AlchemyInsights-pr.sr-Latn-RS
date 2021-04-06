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
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instaliranje sistema Office i usluge OneDrive na Windows virtuelnoj radnoj površini

1. [Priprema i prilagođavanje master VHD slike](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Kreirajte virtuelnu mašinu (VM) ako već nije kreirana.

1. [Instalirajte Office u režimu aktivacije deljenog računara.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Aktivacija deljenog računara omogućava većem broju korisnika da pristupe office programu.

1. [Instalirajte OneDrive u režimu po računaru.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) Obično se OneDrive instalira po korisniku, ali ovde bi trebalo da se instalira po računaru.