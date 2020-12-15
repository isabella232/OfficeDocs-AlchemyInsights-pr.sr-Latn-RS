---
title: Port Google Chrome proširenja na Microsoft Edge (hromozoma)
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
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678983"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="07f16-102">Port Google Chrome proširenja na Microsoft Edge (hromozoma)</span><span class="sxs-lookup"><span data-stu-id="07f16-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="07f16-103">Možete lako da [Priključis Google Chrome proširenja na Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="07f16-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="07f16-104">U većini slučajeva, potrebne su samo minimalne promene da bi se pokrenuli ovi proširenja na lokaciji Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="07f16-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="07f16-105">Tasterske prečice za proširenje i manifestu koje podržava Google Chrome imaju kompatibilan kôd pomoću usluge Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="07f16-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="07f16-106">Međutim, Microsoft Edge ne podržava hromirani APIs. GCM, hroma. identitet. Getacbroj, Chrome. identitet. getAuthToken i Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="07f16-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>