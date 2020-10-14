---
title: Promena e-adrese Microsoft 365 grupe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/10/2020
ms.locfileid: "48462056"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="d7fc9-102">Promena e-adrese grupe Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d7fc9-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="d7fc9-103">Možete da promenite e-adresu grupe Microsoft 365 pomoću centra administracije.</span><span class="sxs-lookup"><span data-stu-id="d7fc9-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="d7fc9-104">Samo izaberite grupu i izaberite @edit e-adresu.</span><span class="sxs-lookup"><span data-stu-id="d7fc9-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="d7fc9-105">Možete da koristite i sledeće komande EXO PowerShell da biste promenili primarnu SMTP adresu Microsoft 365 grupe:</span><span class="sxs-lookup"><span data-stu-id="d7fc9-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="d7fc9-106">Primer</span><span class="sxs-lookup"><span data-stu-id="d7fc9-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
