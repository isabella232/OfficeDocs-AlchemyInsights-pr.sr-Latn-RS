---
title: Korišćenje osnovnih bezbednosnih osnovnih podataka za konfigurisanje operativnog sistema Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696380"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="b2df5-102">Korišćenje Microsoft Intune Security Base za konfigurisanje Windows 10 uređaja</span><span class="sxs-lookup"><span data-stu-id="b2df5-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="b2df5-103">Umetanje bezbednosnih osnovnih funkcija pomaže u zaštiti korisnika i uređaja.</span><span class="sxs-lookup"><span data-stu-id="b2df5-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="b2df5-104">Osnovne bezbednosti zaštite su preliminarne grupe koje se koriste za primenu poznate grupe postavki i podrazumevanih vrednosti koje preporučuje relevantni bezbednosni timovi.</span><span class="sxs-lookup"><span data-stu-id="b2df5-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="b2df5-105">Kreiranjem profila osnovne bezbednosti u Intune kreiraćete predložak koji se sastoji od profila za konfiguraciju sa više uređaja.</span><span class="sxs-lookup"><span data-stu-id="b2df5-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="b2df5-106">Kada primenite bezbednosne osnovne linije na grupe korisnika ili uređaja, postavke se primenjuju na uređaje koji se pokreću u operativnom sistemu Windows 10 ili novijim verzijama.</span><span class="sxs-lookup"><span data-stu-id="b2df5-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="b2df5-107">Na primer, sigurnosna linija bezbednosti Microsoft mobilnog uređaja (MDM) automatski (1) omogućava BitLocker na prenosivim diskovima (2) zahteva lozinku za poništavanje zaključavanja uređaja i (3) onemogućava osnovnu potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="b2df5-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="b2df5-108">Kada podrazumevana vrednost ne radi u okruženju, možete da prilagodite osnovnu liniju da biste primenili postavke koje su vam potrebne.</span><span class="sxs-lookup"><span data-stu-id="b2df5-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="b2df5-109">Osnovne bezbednosne vrednosti takođe pomažu da se uspostavi sigurnosni tok posla koji se završava u usluzi Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b2df5-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="b2df5-110">Slede neke beneficije ove funkcionalnosti:</span><span class="sxs-lookup"><span data-stu-id="b2df5-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="b2df5-111">Osnovna osnova bezbednosti obuhvata najbolje prakse i preporuke za postavke koje utiču na bezbednost.</span><span class="sxs-lookup"><span data-stu-id="b2df5-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="b2df5-112">Zato što Intune partnere sa bezbednosnim timom za Windows koji kreira osnovne linije za smernice grupe, ove preporuke su zasnovane na čvrstim vođstvima i široko iskustvo.</span><span class="sxs-lookup"><span data-stu-id="b2df5-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="b2df5-113">Ako ste novi za podešavanje i nesigurnu odakle da počnete, osnovne bezbednosti će vam pomoći da brzo kreirate i primenite bezbedni profil.</span><span class="sxs-lookup"><span data-stu-id="b2df5-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="b2df5-114">Ako trenutno koristite smernice grupe, a zatim Migriranje u Intune za potrebe upravljanja mnogo je lakše sa bezbednosnim osnovnim linijama, zato što su ove osnovne bezbednosti ugrađene u Intune i sadrže najsavremenije mogućnosti za upravljanje.</span><span class="sxs-lookup"><span data-stu-id="b2df5-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="b2df5-115">Više informacija potražite u članku [Windows bezbednosne osnovne linije](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i [upravljanje mobilnim uređajima](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="b2df5-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>