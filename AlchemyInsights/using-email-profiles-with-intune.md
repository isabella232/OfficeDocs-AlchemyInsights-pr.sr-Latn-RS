---
title: Korišćenje profila e-pošte sa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653302"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="d27a8-102">Korišćenje profila e-pošte sa Intune</span><span class="sxs-lookup"><span data-stu-id="d27a8-102">Using email profiles with Intune</span></span>

<span data-ttu-id="d27a8-103">Intune se mogu koristiti za kreiranje i primenu profila e-pošte za poreklom (ugrađeni) klijent e-pošte na više platformi uređaja.</span><span class="sxs-lookup"><span data-stu-id="d27a8-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="d27a8-104">Informacije o nekom od ograničenja koja se odnose na profile e-pošte, uključujući kako se rukuje prisutnost postojećeg profila i kako da uklonite profile e-pošte, potražite [u članku Dodavanje postavki e-pošte u uređaje pomoću Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="d27a8-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="d27a8-105">Više informacija o tome kako da kreirate profile e-pošte za svaku platformu uređaja potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="d27a8-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="d27a8-106">Postavke Android uređaja da biste konfigurisali e-poštu, potvrdu identiteta i sinhronizaciju u Intune</span><span class="sxs-lookup"><span data-stu-id="d27a8-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="d27a8-107">Dodavanje postavki e-pošte za iOS i iPadOS uređaje u usluzi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d27a8-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="d27a8-108">Postavke profila e-pošte u programu Microsoft Intune za uređaje koje koriste Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="d27a8-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="d27a8-109">Postavke profila e-pošte za uređaje koji rade pod operativnim sistemom Windows 10 u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d27a8-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="d27a8-110">**Uobičajeni problem sa sinhronizacijom**</span><span class="sxs-lookup"><span data-stu-id="d27a8-110">**Common syncing issue**</span></span>

<span data-ttu-id="d27a8-111">**KNOX na Android profilu e-pošte sprečava korisnike, kalendar i zadatke da se sinhronizuju sa korisničkim uređajima.**</span><span class="sxs-lookup"><span data-stu-id="d27a8-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="d27a8-112">Profil e-pošte na Android KNOX-u pruža programu administrator opciju da odluči koji tipovi sadržaja se sinhronizuju sa uređajem tako što će se podesiti svako omogućen.</span><span class="sxs-lookup"><span data-stu-id="d27a8-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="d27a8-113">Ako je postavka za bilo koji tip sadržaja podešena tako da **ne bude podešena** (podrazumevano), taj tip sadržaja se ne sinhronizuje automatski.</span><span class="sxs-lookup"><span data-stu-id="d27a8-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="d27a8-114">Korisnik može da omogući ručno željeni tip sadržaja, ali ta konfiguracija se zamenjuje pomoću postavke Intune, a sinhronizacija prestaje za taj tip sadržaja.</span><span class="sxs-lookup"><span data-stu-id="d27a8-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

