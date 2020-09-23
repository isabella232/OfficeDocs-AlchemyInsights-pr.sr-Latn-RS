---
title: 726 blokira Prosleđivanje e-pošte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219869"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="6f091-102">Blokiranje ili deblokiranje prosleđivanja e-pošte</span><span class="sxs-lookup"><span data-stu-id="6f091-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="6f091-103">Da biste omogućili ili onemogućili Prosleđivanje e-pošte za određeno poštansko sanduče, pogledajte članak [Konfigurisanje prosleđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="6f091-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="6f091-104">Na nivou zakupca kontrola spoljnog prosleđivanja se obavlja pomoću izlazne smernice za borbu protiv bezvredne pošte.</span><span class="sxs-lookup"><span data-stu-id="6f091-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="6f091-105">Ako je podešena na stavku isključeno ili automatski, to može da blokira Prosleđivanje e-pošte pomoću stavke "550 5.7.520 pristup nije dozvoljen, organizacija ne dozvoljava grešku spoljne prosleđivanja".</span><span class="sxs-lookup"><span data-stu-id="6f091-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="6f091-106">Zatim, ako je podešeno da bude blokirano, to je greška koju će korisnici videti.</span><span class="sxs-lookup"><span data-stu-id="6f091-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="6f091-107">Ako je prosleđivanje blokirano, proverite da li su smernice konfigurisane tako da omogućavaju eksterni Autonapred.</span><span class="sxs-lookup"><span data-stu-id="6f091-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="6f091-108">Možete da potvrdite smernice za filtriranje odlazne bezvredne pošte iz centra za bezbednost i usaglašenost ili tako što ćete pokrenuti komandnu karticu. ime za for, Autoforwardingmod.</span><span class="sxs-lookup"><span data-stu-id="6f091-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="6f091-109">Ako želite da podesite automatsko blokiranje, ista komanda će vam odmah reći stanje politike.</span><span class="sxs-lookup"><span data-stu-id="6f091-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="6f091-110">Napomena: preporučuje se da spoljna automatska funkcija ostane sprečena u podrazumevanim smernicama za izlazne količine i omogućite samo za korisnike kojima je potrebna spoljna prosleđivanje kreiranjem prilagođenih smernica za te korisnike.</span><span class="sxs-lookup"><span data-stu-id="6f091-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="6f091-111">Možete pročitati više o [konfigurisanju spoljnog prosleđivanja e-pošte u sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="6f091-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>