---
title: Upravljanje sinhronizovanim korisnikom
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823981"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="0af7e-102">Nije moguće podesiti primarnu adresu e-pošte, promeniti atribute korisnika ili ukloniti/izbrisati sinhronizovanog korisnika</span><span class="sxs-lookup"><span data-stu-id="0af7e-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="0af7e-103">Ako je sinhronizacija direktorijuma omogućena za okruženje, neki atributi korisnika ili objekta ne mogu da se promene pomoću Microsoft 365 centra za atribute.</span><span class="sxs-lookup"><span data-stu-id="0af7e-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="0af7e-104">Da biste u potpunosti upravljali sinhronizovanim korisnicima i svim njihovim atributima, koristite lokalne active directory korisnike i konzolu za upravljanje grupama (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="0af7e-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="0af7e-105">Druga mogućnost je da promenite pojedinačne korisnike ili atribute za sinhronizovane korisnike pomoću programa powershell, kao što je prikazano u ovim uobičajenim primerima:</span><span class="sxs-lookup"><span data-stu-id="0af7e-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
