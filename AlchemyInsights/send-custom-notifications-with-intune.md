---
title: Slanje prilagođenih obaveštenja Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720660"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="1a7d1-102">Kako da pošaljete prilagođena obaveštenja korisnicima kompletnih iOS i Android uređaja</span><span class="sxs-lookup"><span data-stu-id="1a7d1-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="1a7d1-103">Prilagođena obaveštenja za Intune obrađuje aplikacija portal preduzeća na uređaju korisnika.</span><span class="sxs-lookup"><span data-stu-id="1a7d1-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="1a7d1-104">Aplikacija zatim kreira obaveštenje o pritiskom na tom uređaju.</span><span class="sxs-lookup"><span data-stu-id="1a7d1-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="1a7d1-105">Slede preduslovi za podršku prilikom prijema prilagođenih obaveštenja, a zatim za aplikaciju da biste zatim kreirali obaveštenje o pritisanju:</span><span class="sxs-lookup"><span data-stu-id="1a7d1-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="1a7d1-106">Uređaj mora da ima instaliran aplikaciju za preduzeće portal.</span><span class="sxs-lookup"><span data-stu-id="1a7d1-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="1a7d1-107">Uređaj mora da omogući aplikaciji portala preduzeća da šalje push obaveštenja.</span><span class="sxs-lookup"><span data-stu-id="1a7d1-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="1a7d1-108">Kada se aplikacija instalira ili ažurira, on će zatražiti od korisnika da dozvoli obaveštenja.</span><span class="sxs-lookup"><span data-stu-id="1a7d1-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="1a7d1-109">Android uređaji mora da imaju instalirane Google Play usluge.</span><span class="sxs-lookup"><span data-stu-id="1a7d1-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="1a7d1-110">Uređaj mora biti upisan u Intune.</span><span class="sxs-lookup"><span data-stu-id="1a7d1-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="1a7d1-111">Više informacija o tome kako da pošaljete poruku potražite u [dokumentaciji funkcije](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="1a7d1-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
