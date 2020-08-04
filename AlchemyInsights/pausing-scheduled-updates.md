---
title: Pauziranje planiranih ispravki
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555988"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="0d584-102">Pauziranje planiranih ispravki</span><span class="sxs-lookup"><span data-stu-id="0d584-102">Pausing scheduled updates</span></span>

<span data-ttu-id="0d584-103">Kada se izda komanda za Pauziranje, uređaji ne obrađuju komandu sve dok sledeći put ne prijavite u Intune.</span><span class="sxs-lookup"><span data-stu-id="0d584-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="0d584-104">Zbog ovoga, uređaji mogu imati:</span><span class="sxs-lookup"><span data-stu-id="0d584-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="0d584-105">Instalirali planirane dopune pre nego što se prijavite.</span><span class="sxs-lookup"><span data-stu-id="0d584-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="0d584-106">Isključen kada ste izdali komandu "Pauziraj".</span><span class="sxs-lookup"><span data-stu-id="0d584-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="0d584-107">U ovom slučaju, kada je uređaj uključen, možda su preuzeli i instalirali planirane dopune pre nego što je prijavite.</span><span class="sxs-lookup"><span data-stu-id="0d584-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>