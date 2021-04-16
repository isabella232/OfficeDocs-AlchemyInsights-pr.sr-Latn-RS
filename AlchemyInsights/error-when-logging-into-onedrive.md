---
title: 0x8004de40 greške prilikom pokretanja oneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813666"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="d155f-102">0x8004de40 greške prilikom pokretanja oneDrive</span><span class="sxs-lookup"><span data-stu-id="d155f-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="d155f-103">Ako dobijete poruku o **grešci 0x8004de40** se pri prijavci u OneDrive, ponovootkucajte računar dok ste povezani sa poslovnim ili školskim domenom.</span><span class="sxs-lookup"><span data-stu-id="d155f-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="d155f-104">Ako dobijete ovu grešku nakon ponošanja, pokušajte ovo dok ste povezani sa poslovnim ili školskim domenom:</span><span class="sxs-lookup"><span data-stu-id="d155f-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="d155f-105">Kliknite na dugme Start i  u polju za pretragu otkucajte **cmd** ili komandnu liniju, kliknite desnim tasterom miša na aplikaciju komandne linije i izaberite stavku Pokreni **kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="d155f-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="d155f-106">Ako budete upitani za administratorsku lozinku ili za potvrdu, otkucajte lozinku ili kliknite na dugme **Dozvoli.**</span><span class="sxs-lookup"><span data-stu-id="d155f-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="d155f-107">U prozoru komandne linije otkucajte **dsregcmd /leave**  i sačekajte da se komanda dovrši.</span><span class="sxs-lookup"><span data-stu-id="d155f-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="d155f-108">Zatim **otkucajte dsregcmd /join** i sačekajte da se komanda dovrši.</span><span class="sxs-lookup"><span data-stu-id="d155f-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="d155f-109">Ponovo poništite računar.</span><span class="sxs-lookup"><span data-stu-id="d155f-109">Reboot your computer.</span></span>
