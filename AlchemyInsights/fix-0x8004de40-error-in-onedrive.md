---
title: Otklonite 0x8004de40 greške u usluzi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649762"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="fd53c-102">Otklonite 0x8004de40 greške u usluzi OneDrive</span><span class="sxs-lookup"><span data-stu-id="fd53c-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="fd53c-103">Ako imate Windows 7 i dobijate ovu grešku, ažurirajte je da biste omogućili [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao podrazumevane bezbedne protokole u operativnom sistemu WinHTTP u operativnom sistemu Windows.</span><span class="sxs-lookup"><span data-stu-id="fd53c-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="fd53c-104">Ako imate Windows 10 i dobijate 0x8004de40 sa OneDrive:</span><span class="sxs-lookup"><span data-stu-id="fd53c-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="fd53c-105">Ponovo poništite računar na koji to utiče dok ste povezani sa Acitve Directory domenom.</span><span class="sxs-lookup"><span data-stu-id="fd53c-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="fd53c-106">Ako poništavanje ne reši problem, ponovo se pridružite uređaju iz usluge Azure AD i ponovo se pridružite uređaju.</span><span class="sxs-lookup"><span data-stu-id="fd53c-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="fd53c-107">**Napomi:** Trebalo bi da budete na mreži preduzeća dok izvršavate ove korake.</span><span class="sxs-lookup"><span data-stu-id="fd53c-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="fd53c-108">Nemojte da izvršite ove korake kada niste povezani sa infrastrukturom preduzeća (na primer, prilikom putovanja).</span><span class="sxs-lookup"><span data-stu-id="fd53c-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="fd53c-109">Otvorite komandnu liniju sa punim privilegijama tako što ćete izabrati start **,** kliknite desnim tasterom miša na stavku **Komandna** linija , a zatim izaberite **stavku Pokreni kao administrator**.</span><span class="sxs-lookup"><span data-stu-id="fd53c-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="fd53c-110">Otkucajte *dsregcmd /leave* i pritisnite **taster Enter**.</span><span class="sxs-lookup"><span data-stu-id="fd53c-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="fd53c-111">Kada završite, *otkucajte dsregcmd /join i* pritisnite **taster Enter.**</span><span class="sxs-lookup"><span data-stu-id="fd53c-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="fd53c-112">Kada se dovrše, zatvorite komandnu liniju.</span><span class="sxs-lookup"><span data-stu-id="fd53c-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="fd53c-113">Ponovo poništite računar i prijavite se u OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fd53c-113">Reboot the computer, and log into OneDrive.</span></span>