---
title: Kako da onemogućite spoljne grupe
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704142"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="89da3-102">Kako da onemogućite spoljne grupe</span><span class="sxs-lookup"><span data-stu-id="89da3-102">How to disable External Groups</span></span>

<span data-ttu-id="89da3-103">Yammer spoljna razmena poruka primenjuje Exchange pravila transporta (ETRs), skupa proaktivnih kontrola radi sprečavanja deljenja informacija o preduzeću.</span><span class="sxs-lookup"><span data-stu-id="89da3-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="89da3-104">Da biste ograničili korisnike da kreiraju spoljne grupe, treba da konfigurišete pravilo za razmenu Exchange servera (ETR), a zatim da konfigurišete Yammer da koristi pravilo Exchange transporta za blokiranje spoljnih poruka.</span><span class="sxs-lookup"><span data-stu-id="89da3-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="89da3-105">Kada kreirate pravilo u Exchange online centru administracije, slijedite ove korake da biste konfigurisali ETR da se primenjuje u usluzi Yammer:</span><span class="sxs-lookup"><span data-stu-id="89da3-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="89da3-106">Prijavite se na Yammer kao verifikovan administrator i u **Yammer centru administracije** **Izaberite stavku \> Postavke sadržaja C i bezbednosti.**</span><span class="sxs-lookup"><span data-stu-id="89da3-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="89da3-107">U okviru **spoljna razmena poruka**, izaberite **primenu primene Exchange online Exchange pravila transporta (etrs) u usluzi Yammer.**</span><span class="sxs-lookup"><span data-stu-id="89da3-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="89da3-108">Odaberite stavku **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="89da3-108">Choose **Save**.</span></span>

<span data-ttu-id="89da3-109">Više informacija potražite u članku [Onemogućavanje spoljnih poruka u Yammer mreži](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="89da3-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  