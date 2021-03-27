---
title: Automatsko prijavljivanje u Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398743"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="11eed-102">Automatsko prijavljivanje u Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="11eed-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="11eed-103">Microsoft Edge koristi podrazumevani OS nalog za automatsko prijavljivanje korisnika u skladu sa načinom konfigurisanja uređaja korisnika.</span><span class="sxs-lookup"><span data-stu-id="11eed-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="11eed-104">Scenariji svakog tipa konfiguracije uređaja i procesa zavisnog korisnika su opisani u nastavku:</span><span class="sxs-lookup"><span data-stu-id="11eed-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="11eed-105">**Uređaj je hibridni/AAD-J:** Ova opcija je dostupna u operativnom sistemu Windows 10, operativnom sistemu Windows sa nižim nivoom i odgovarajućim verzijama servera.</span><span class="sxs-lookup"><span data-stu-id="11eed-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="11eed-106">Korisnici se automatski prilaže svojim Azure Active Directory (AD)nalozima.</span><span class="sxs-lookup"><span data-stu-id="11eed-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="11eed-107">**Uređaj je pridružen domenu:** Ova opcija je dostupna u operativnom sistemu Windows 10, operativnom sistemu Windows sa nižim nivoom i odgovarajućim verzijama servera.</span><span class="sxs-lookup"><span data-stu-id="11eed-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="11eed-108">Prema podrazumevanim postavkama, korisnici sa nalozima domena nisu automatski prijavljeni; da biste omogućili automatsko prijavljivanje za njih, koristite **smernicu ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="11eed-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="11eed-109">Da biste omogućili automatsko prijavljivanje za korisnike koji imaju Azure AD naloge, razmotrite hibridno pridruživanje uređajima.</span><span class="sxs-lookup"><span data-stu-id="11eed-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="11eed-110">Podrazumevani nalog operativnog sistema je **Microsoft** nalog: Ova opcija je dostupna u operativnom sistemu Windows 10 RS3 (verzija 1709, verzija 10.0.16299) i novijim verzijama.</span><span class="sxs-lookup"><span data-stu-id="11eed-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="11eed-111">Malo je verovatno da će se scenario desiti na poslovnim uređajima.</span><span class="sxs-lookup"><span data-stu-id="11eed-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="11eed-112">Međutim, ako je podrazumevani OS nalog Microsoft nalog, Microsoft Edge će se automatski prijaviti korisnika sa Microsoft nalogom.</span><span class="sxs-lookup"><span data-stu-id="11eed-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
