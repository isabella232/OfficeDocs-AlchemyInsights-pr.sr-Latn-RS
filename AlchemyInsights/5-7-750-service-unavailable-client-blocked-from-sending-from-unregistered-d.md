---
title: 1048 5.7.750 usluga nije dostupna. Klijent je blokirao slanje iz neregistrovanih domena
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664256"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="3fb22-103">5.7.750 klijent je blokiran od slanja iz neregistrovanog domena</span><span class="sxs-lookup"><span data-stu-id="3fb22-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="3fb22-104">Greška se javlja kada se velika količina poruka pošalje iz domena koji nisu obezbeđeni u zakupcu (dodata kao prihvaćen i proveren).</span><span class="sxs-lookup"><span data-stu-id="3fb22-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="3fb22-105">Da biste izbegli ovu grešku, možete da koristite konektor toka e-pošte zasnovan na certifikatu gde je domen certifikata obezbeđen domen ili možete da ih dodelite svim domenima za slanje.</span><span class="sxs-lookup"><span data-stu-id="3fb22-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
