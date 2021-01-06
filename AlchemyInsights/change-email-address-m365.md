---
title: Promena e-adrese Microsoft 365 Group ili e-adrese aplikacije Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756571"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="39e0e-102">Promena e-adrese Microsoft 365 Group ili e-adrese aplikacije Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="39e0e-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="39e0e-103">Možete da promenite e-adresu grupe Microsoft 365 Group ili e-adresu aplikacije Microsoft Teams [Microsoft 365 centar administracije](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="39e0e-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="39e0e-104">Samo izaberite grupu i izaberite stavku @uredi e-adresu.</span><span class="sxs-lookup"><span data-stu-id="39e0e-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="39e0e-105">Možete da koristite i sledeće EXO PowerShell komande da biste promenili primarnu SMTP adresu Microsoft 365 grupe/aplikacije Teams:</span><span class="sxs-lookup"><span data-stu-id="39e0e-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="39e0e-106">Primer:</span><span class="sxs-lookup"><span data-stu-id="39e0e-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
