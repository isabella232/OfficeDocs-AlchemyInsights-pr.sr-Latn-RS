---
title: Instaliranje Kancelarija i OneDrive virtuelnoj radnoj površini Windows
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
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028630"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Instaliranje Kancelarija i OneDrive virtuelnoj radnoj površini Windows

1. [Priprema i prilagođavanje master VHD slike](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). Kreirajte virtuelnu mašinu (VM) ako već nije kreirana.

1. [Instalirajte Kancelarija u režimu aktivacije deljenog računara.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Aktivacija deljenog računara omogućava većem broju korisnika da pristupe Kancelarija.

1. [Instalirajte OneDrive u režimu po računaru.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) Obično se OneDrive instalira po korisniku, ali ovde bi trebalo da se instalira po računaru.