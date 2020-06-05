---
title: Promena e-adrese Microsoft 365 grupe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580671"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="a1085-102">Promena e-adrese Microsoft 365 grupe</span><span class="sxs-lookup"><span data-stu-id="a1085-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="a1085-103">E-adresu Microsoft 365 grupe možete da promenite pomoću administratorskog centra.</span><span class="sxs-lookup"><span data-stu-id="a1085-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="a1085-104">Samo izaberite grupu i izaberite @edit e-adresu.</span><span class="sxs-lookup"><span data-stu-id="a1085-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="a1085-105">Takođe možete koristiti sledeću komandu "EXO PowerShell" da biste promenili primarnu SMTP adresu Microsoft 365 grupe:</span><span class="sxs-lookup"><span data-stu-id="a1085-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="a1085-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="a1085-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="a1085-107">Primer:</span><span class="sxs-lookup"><span data-stu-id="a1085-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
