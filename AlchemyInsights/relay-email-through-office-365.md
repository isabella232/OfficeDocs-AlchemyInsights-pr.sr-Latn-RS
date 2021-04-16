---
title: Razmena e-pošte putem sistema Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809669"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="c3d00-102">Kako da podesite višefunkcionalni uređaj ili aplikaciju za slanje e-pošte</span><span class="sxs-lookup"><span data-stu-id="c3d00-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="c3d00-103">Da biste saznali koje opcije imate i koje korake treba da izvršite, pogledajte članak [Kako da podesite višefunkcionalni uređaj ili aplikaciju za slanje e-pošte pomoću sistema Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="c3d00-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="c3d00-104">**Napomena:** ako imate uređaj ili aplikaciju koja je nedavno prestala sa radom, imajte na umu da smo nedavno počeli planirano [onemogućavanje 3DES šifrovanja](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption).</span><span class="sxs-lookup"><span data-stu-id="c3d00-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="c3d00-105">Da biste videli pogođene uređaje, idite na [Izveštaj o klijentima SMTP potvrde identiteta](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="c3d00-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="c3d00-106">Uobičajene greške koje se mogu javiti: Neuspešna provera identiteta, TLS otkazivanje/greška, greške u algoritmu za šifrovanje, algoritmi koji se ne podudaraju ili prekinuta veza.</span><span class="sxs-lookup"><span data-stu-id="c3d00-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="c3d00-107">Da rešite problem:</span><span class="sxs-lookup"><span data-stu-id="c3d00-107">To resolve the issue:</span></span>

 - <span data-ttu-id="c3d00-108">**Windows Server 2003 IIS SMTP neće više funkcionisati – potrebna je novija verzija operativnog sistema Windows.**</span><span class="sxs-lookup"><span data-stu-id="c3d00-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="c3d00-109">Obratite se dobavljaču aplikacije ili uređaja da biste videli da li je podržana moderna metoda šifrovanja ili da li postoji ispravka.</span><span class="sxs-lookup"><span data-stu-id="c3d00-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
