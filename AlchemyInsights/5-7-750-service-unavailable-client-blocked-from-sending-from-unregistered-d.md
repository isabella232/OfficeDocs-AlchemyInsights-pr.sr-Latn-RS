---
title: 1048 5.7.750 Usluga nije dostupna. Klijent je blokiran za slanje sa neregisterednih domena
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
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774265"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="01904-103">5.7.750 Klijent je blokiran slanje sa neregistranog domena</span><span class="sxs-lookup"><span data-stu-id="01904-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="01904-104">Do ove greške dolazi kada se velika količina poruka šalje sa domena koji nisu obezbeđeni u vašem zakuatoru (dodati kao prihvaćeni domeni i proverena je valjanost).</span><span class="sxs-lookup"><span data-stu-id="01904-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="01904-105">Da biste izbegli ovu grešku, možete da koristite konektor protoka pošte zasnovan na certifikatu, gde je domen certifikata domen obezbeđen ili možete da obezbede sve domene za slanje.</span><span class="sxs-lookup"><span data-stu-id="01904-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="01904-106">Više informacija potražite u temi Rešavanje problema sa isporukom e-pošte za kodove greške od [5.7.700 do 5.7.750 u e-Exchange Online.](https://go.microsoft.com/fwlink/?linkid=2164955)</span><span class="sxs-lookup"><span data-stu-id="01904-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>