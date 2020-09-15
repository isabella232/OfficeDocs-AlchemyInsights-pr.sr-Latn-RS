---
title: Rad sa ličnim ID-ovi za iOS VIP aplikacije 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688960"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="76ddf-102">Rad sa iOS VANP aplikacijama</span><span class="sxs-lookup"><span data-stu-id="76ddf-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="76ddf-103">Pročitajte [Kako da upravljate iOS aplikacijama kupljenim kroz program za disk jedinicu pomoću programa Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) da biste saznali više o funkcijama, ograničenjima i koracima za korišćenje Apple programa za kupovinu volumena i podrške za njega u Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="76ddf-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="76ddf-104">**Uobičajeni problemi:** "Za korisnike sam dodelila iOS VIPP aplikaciju, ali Instalacija nije uspela".</span><span class="sxs-lookup"><span data-stu-id="76ddf-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="76ddf-105">To se može dogoditi ako se na jednom dobavljaču usluga upravljanja mobilnim uređajima koristi pojedinačni VIPP.</span><span class="sxs-lookup"><span data-stu-id="76ddf-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="76ddf-106">VIP simboli iz Apple se mogu koristiti samo sa jednim dobavljačem.</span><span class="sxs-lookup"><span data-stu-id="76ddf-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="76ddf-107">Ako ste koristili Office Token sa više dobavljača, morate ponovo da otpremate simbol za Intune.</span><span class="sxs-lookup"><span data-stu-id="76ddf-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="76ddf-108">Instalacija takođe može da propadne ako ukupan broj instalacija premašuje broj licenci.</span><span class="sxs-lookup"><span data-stu-id="76ddf-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="76ddf-109">Da biste prikazali izveštaj o korišćenju licenci, idite na stranicu **Intune licence za mobilne aplikacije** \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="76ddf-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="76ddf-110">Da biste saznali kako da povratite licence koristite, pogledajte [Ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="76ddf-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
