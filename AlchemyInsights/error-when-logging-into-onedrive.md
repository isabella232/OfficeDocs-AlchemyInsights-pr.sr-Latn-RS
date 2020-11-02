---
title: Greška 0x8004de40 prilikom pokretanja usluge OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823116"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="7f697-102">Greška 0x8004de40 prilikom pokretanja usluge OneDrive</span><span class="sxs-lookup"><span data-stu-id="7f697-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="7f697-103">Ako primite grešku **0x8004de40** prilikom prijavljivanja u OneDrive, ponovo pokrenite računar dok ste povezani sa poslovnim ili školskim domenom.</span><span class="sxs-lookup"><span data-stu-id="7f697-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="7f697-104">Ako dobijete ovu grešku posle ponovnog pokretanja, isprobajte ovo povezivanje sa poslovnim ili školskim domenom:</span><span class="sxs-lookup"><span data-stu-id="7f697-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="7f697-105">Kliknite na dugme Start i otkucajte **cmd** ili **Komandna linija**  u polju za pretragu, kliknite desnim tasterom miša na aplikaciju komandne linije i izaberite stavku  **Pokreni kao administrator** .</span><span class="sxs-lookup"><span data-stu-id="7f697-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="7f697-106">Ako vam bude zatraženo da dobijete administratorsku lozinku ili za potvrdu, otkucajte lozinku ili kliknite na dugme **Omogući** .</span><span class="sxs-lookup"><span data-stu-id="7f697-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="7f697-107">U prozoru komandne linije otkucajte **dsregcmd/ostavi**  i sačekajte da se komanda dovrši.</span><span class="sxs-lookup"><span data-stu-id="7f697-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="7f697-108">Zatim otkucajte **dsregcmd/JOIN** i sačekajte da se komanda dovrši.</span><span class="sxs-lookup"><span data-stu-id="7f697-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="7f697-109">Ponovo pokrenite računar.</span><span class="sxs-lookup"><span data-stu-id="7f697-109">Reboot your computer.</span></span>
