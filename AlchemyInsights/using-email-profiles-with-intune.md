---
title: Korišćenje profila e-pošte sa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555763"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="b86ac-102">Korišćenje profila e-pošte sa Intune</span><span class="sxs-lookup"><span data-stu-id="b86ac-102">Using email profiles with Intune</span></span>

<span data-ttu-id="b86ac-103">Intune može da se koristi za kreiranje i primenu profila e-pošte za osnovni (ugrađeni) klijent e-pošte na više platformi uređaja.</span><span class="sxs-lookup"><span data-stu-id="b86ac-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="b86ac-104">Informacije o nekim ograničenjima povezanim sa profilima e-pošte, uključujući način na koji se obrađuju prisustvo postojećih profila i kako se uklanjaju Profili e-pošte, pogledajte odeljak [Dodavanje postavki e-pošte na uređaje pomoću funkcije Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="b86ac-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="b86ac-105">Više informacija o kreiranju profila e-pošte za svaku platformu uređaja potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="b86ac-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="b86ac-106">Postavke za Android uređaje da biste konfigurisali e-poštu, potvrdu identiteta i sinhronizaciju u usluzi Intune</span><span class="sxs-lookup"><span data-stu-id="b86ac-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="b86ac-107">Dodavanje postavki e-pošte za iOS i iPadOS uređaje u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b86ac-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="b86ac-108">Postavke profila e-pošte u usluzi Microsoft Intune za uređaje koji rade pod operativnim sistemom Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="b86ac-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="b86ac-109">Postavke profila e-pošte za uređaje koji rade pod operativnim sistemom Windows 10 u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b86ac-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="b86ac-110">**Uobičajeno pitanje sinhronizacije**</span><span class="sxs-lookup"><span data-stu-id="b86ac-110">**Common syncing issue**</span></span>

<span data-ttu-id="b86ac-111">**KNOX na Android e-pošti profil sprečava korisničke kontakte, kalendar i zadatke, od sinhronizacije do korisničkih uređaja.**</span><span class="sxs-lookup"><span data-stu-id="b86ac-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="b86ac-112">Profil e-pošte KNOX na Android KNOX uređaju nudi administratoru opcije da odluči koji tipovi sadržaja se sinhronizuju sa uređajem tako što će podesiti svaki od njih da ih omogući.</span><span class="sxs-lookup"><span data-stu-id="b86ac-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="b86ac-113">Ako je postavka za bilo koji od tipova sadržaja postavljena na vrednost " **Nije konfigurisano** " (podrazumevani), taj tip sadržaja se neće automatski sinhronizovati.</span><span class="sxs-lookup"><span data-stu-id="b86ac-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="b86ac-114">Korisnik će možda omogućiti tip sadržaja koji žele direktno na uređaj, ali ta konfiguracija se zamenjuje postavkom smernica Intune, a sinhronizacija se zaustavlja za taj tip sadržaja.</span><span class="sxs-lookup"><span data-stu-id="b86ac-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

