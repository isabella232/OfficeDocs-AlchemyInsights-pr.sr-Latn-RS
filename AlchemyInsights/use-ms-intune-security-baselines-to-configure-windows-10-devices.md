---
title: Korišćenje Microsoft Intune Base Security za konfigurisanje Windows 10 uređaja
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573532"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="87291-102">Korišćenje Microsoft Intune Base Security za konfigurisanje Windows 10 uređaja</span><span class="sxs-lookup"><span data-stu-id="87291-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="87291-103">Umetanje bezbednosnih osnovnih funkcija pomaže u zaštiti korisnika i uređaja.</span><span class="sxs-lookup"><span data-stu-id="87291-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="87291-104">Osnovne bezbednosti zaštite su preliminarne grupe koje se koriste za primenu poznate grupe postavki i podrazumevanih vrednosti koje preporučuje relevantni bezbednosni timovi.</span><span class="sxs-lookup"><span data-stu-id="87291-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="87291-105">Kreiranjem profila osnovne bezbednosti u Intune kreiraćete predložak koji se sastoji od profila za konfiguraciju sa više uređaja.</span><span class="sxs-lookup"><span data-stu-id="87291-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="87291-106">Kada primenite bezbednosne osnovne linije na grupe korisnika ili uređaja, postavke se primenjuju na uređaje koji se pokreću u operativnom sistemu Windows 10 ili novijim verzijama.</span><span class="sxs-lookup"><span data-stu-id="87291-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="87291-107">Na primer, komanda "MDM Security" automatski (1) omogućava BitLocker za prenosive diskove, (2) zahteva lozinku za poništavanje zaključavanja uređaja i (3) onemogućava osnovnu potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="87291-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="87291-108">Kada podrazumevana vrednost ne radi u okruženju, prilagodite osnovnu liniju da biste primenili postavke koje su vam potrebne.</span><span class="sxs-lookup"><span data-stu-id="87291-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="87291-109">Osnovne bezbednosne vrednosti takođe pomažu da se uspostavi sigurnosni tok posla koji se završava u usluzi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="87291-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="87291-110">Slede neke beneficije:</span><span class="sxs-lookup"><span data-stu-id="87291-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="87291-111">Osnovna osnova bezbednosti obuhvata najbolje prakse i preporuke za postavke koje utiču na bezbednost.</span><span class="sxs-lookup"><span data-stu-id="87291-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="87291-112">Zato što Intune partnere sa bezbednosnim timom za Windows koji kreira osnovne linije za smernice grupe, ove preporuke su zasnovane na čvrstim vođstvima i široko iskustvo.</span><span class="sxs-lookup"><span data-stu-id="87291-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="87291-113">Ako ste novi za podešavanje i nesigurnu odakle da počnete, osnovne bezbednosti će vam pomoći da brzo kreirate i primenite bezbedni profil.</span><span class="sxs-lookup"><span data-stu-id="87291-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="87291-114">Ako trenutno koristite smernice grupe, a zatim Migriranje u Intune za potrebe upravljanja mnogo je lakše sa bezbednosnim osnovnim linijama, zato što su ugrađene u Intune i sadrže najsavremenije mogućnosti za upravljanje.</span><span class="sxs-lookup"><span data-stu-id="87291-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="87291-115">Da biste saznali više, pogledajte članak [Windows Security osnovni](https://go.microsoft.com/fwlink/?linkid=2141503) [Uređaji i upravljanje mobilnim uređajima](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="87291-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>