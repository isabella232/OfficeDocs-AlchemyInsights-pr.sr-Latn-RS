---
title: Omogućavanje nadgledanja poštanskog sandučeta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806305"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="d9f4b-102">Omogućavanje nadgledanja poštanskog sandučeta</span><span class="sxs-lookup"><span data-stu-id="d9f4b-102">Enable mailbox auditing</span></span>

<span data-ttu-id="d9f4b-103">Da biste omogućili nadgledanje poštanskog sandučeta za jednog korisnika ili za celu organizaciju, sledeće cmdlet lokacije moraju da se pokrenu sa udaljenog programskog sistema Power Shell:</span><span class="sxs-lookup"><span data-stu-id="d9f4b-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="d9f4b-104">**Pojedinačni korisnik**</span><span class="sxs-lookup"><span data-stu-id="d9f4b-104">**Single User**</span></span>
  
<span data-ttu-id="d9f4b-105">Scenofor-poštansko sanduče-identitet "Džejn Dau" $true</span><span class="sxs-lookup"><span data-stu-id="d9f4b-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="d9f4b-106">**Kompanija**</span><span class="sxs-lookup"><span data-stu-id="d9f4b-106">**Organization**</span></span>
  
<span data-ttu-id="d9f4b-107">Nabavite-poštansko sanduče – Rezultućete neograničeno-Filtriraj {RecipientTypeDetails-EQ "Korisničkopoštansko sanduče"} | Scenofor-poštansko sanduče – $true</span><span class="sxs-lookup"><span data-stu-id="d9f4b-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="d9f4b-108">uči više</span><span class="sxs-lookup"><span data-stu-id="d9f4b-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

