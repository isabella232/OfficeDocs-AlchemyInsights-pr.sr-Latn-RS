---
title: Koristite Microsoft Intune bezbednosti da biste konfigurisali Windows 10 uređaje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794131"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="2b78c-102">Koristite Microsoft Intune bezbednosti da biste konfigurisali Windows 10 uređaje</span><span class="sxs-lookup"><span data-stu-id="2b78c-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="2b78c-103">Bezbednosne linije usluge Intune pomažu u zaštiti korisnika i uređaja.</span><span class="sxs-lookup"><span data-stu-id="2b78c-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="2b78c-104">Osnove bezbednosti su Windows postavki unapred konfigurisanih grupa koje se koriste za primenu poznate grupe postavki i podrazumevanih vrednosti koje preporučuju relevantni timovi za bezbednost.</span><span class="sxs-lookup"><span data-stu-id="2b78c-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="2b78c-105">Kreiranjem profila sa osnovnim linijama bezbednosti u programu Intune kreirate predložak koji se sastoji od više profila za konfiguraciju uređaja.</span><span class="sxs-lookup"><span data-stu-id="2b78c-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="2b78c-106">Kada primenite osnovne linije bezbednosti na grupe korisnika ili uređaja, postavke se primenjuju na uređaje koji se Windows 10 ili kasnije.</span><span class="sxs-lookup"><span data-stu-id="2b78c-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="2b78c-107">Na primer, bezbednosna linija za upravljanje Microsoft mobilnim uređajima (MDM) automatski omogućava da BitLocker prenosive disk jedinice, zahteva lozinku za otključavanje uređaja, a onemogućava osnovnu potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="2b78c-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="2b78c-108">Kada podrazumevana vrednost ne funkcioniše za okruženje, možete da prilagodite osnovnu liniju da biste primenili postavke koje su vam potrebne.</span><span class="sxs-lookup"><span data-stu-id="2b78c-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="2b78c-109">Bezbednosne osnovne linije takođe pomažu u uspostavljanju sveobdnog bezbednog toka posla u Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2b78c-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="2b78c-110">Bezbednosna osnovna linija sadrži najbolje prakse i preporuke za postavke koje utiču na bezbednost.</span><span class="sxs-lookup"><span data-stu-id="2b78c-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="2b78c-111">Intune partneri sa Windows za bezbednost koji pravi osnovne linije za smernice grupe, tako da se ove preporuke zasnivaju na solid smernicama i obimnom iskustvu.</span><span class="sxs-lookup"><span data-stu-id="2b78c-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="2b78c-112">Ako ste novi korisnik usluge Intune i niste sigurni odakle da počnete, osnovne linije bezbednosti vam pomažu da brzo napravite i primenite bezbedan profil.</span><span class="sxs-lookup"><span data-stu-id="2b78c-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="2b78c-113">Ako trenutno koristite smernice grupe, migracija u Intune u svrhe upravljanja mnogo je lakša sa osnovnim linijama bezbednosti jer su ugrađene u intune i obuhvataju mogućnosti upravljanja isecanjem ivica.</span><span class="sxs-lookup"><span data-stu-id="2b78c-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="2b78c-114">Da biste saznali više, pogledajte [Windows osnove bezbednosti i](/windows/security/threat-protection/windows-security-baselines) Upravljanje [mobilnim uređajima.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="2b78c-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

