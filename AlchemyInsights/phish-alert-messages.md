---
title: 2491 upozoravanje e-poruka iz "Phish isporučene zbog smernica zakupca ili zamene korisnika"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728625"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="55004-102">Upozoravanje e-poruka iz ' Phish isporučene zbog polise zakupca ili korisnika</span><span class="sxs-lookup"><span data-stu-id="55004-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="55004-103">Podrazumevana smernica za obaveštenje pod imenom "Phish isporučen zbog zakupca ili zamene korisnika" je poslata zakupcima Office 365 ATP P1 i P2 licenci.</span><span class="sxs-lookup"><span data-stu-id="55004-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="55004-104">Ako ste dobili ovo obaveštenje, evo koraka za istraživanje:</span><span class="sxs-lookup"><span data-stu-id="55004-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="55004-105">U poruci upozorenja kliknite na dugme **Prikaži obaveštenje** da biste otiљli na stranicu **obaveštenja** u centru za bezbednost & bezbednosti.</span><span class="sxs-lookup"><span data-stu-id="55004-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="55004-106">Potvrdite izbor u polju za potvrdu obaveštenje da biste videli opciju za **prikaz liste poruka** ili **prikazali poruke u programu Explorer**.</span><span class="sxs-lookup"><span data-stu-id="55004-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="55004-107">Obe opcije vas vodi do detalja poruke, što obuhvata ID poruke.</span><span class="sxs-lookup"><span data-stu-id="55004-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="55004-108">Imajte u vidu da će karika u programu Explorer za pretnju automatski filtrirati poruke koje se podudaraju sa kriterijumima obaveštenja.</span><span class="sxs-lookup"><span data-stu-id="55004-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="55004-109">Možda ćete morati da prilagodite filter datuma u istraživaču pretnji.</span><span class="sxs-lookup"><span data-stu-id="55004-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="55004-110">Phishing poruka je isporučena zbog ručno konfigurisane zamene:</span><span class="sxs-lookup"><span data-stu-id="55004-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="55004-111">Dozvoljeni pošiljalac ili domen koji je postavio korisnik.</span><span class="sxs-lookup"><span data-stu-id="55004-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="55004-112">Dozvoljeni pošiljalac ili domen postavljen u okviru smernica za sprečavanje bezvredne pošte.</span><span class="sxs-lookup"><span data-stu-id="55004-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="55004-113">Dozvoljena IP adresa u smernicama filtriranja veze.</span><span class="sxs-lookup"><span data-stu-id="55004-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="55004-114">Pravilo toka pošte (poznato i kao pravilo transporta) koje je podešeno da omogući poruke.</span><span class="sxs-lookup"><span data-stu-id="55004-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="55004-115">Ako verujete da je poruka pogrešno označena kao frish, koristite [programski dodatak Outlook izveštaj](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) za prosleđivanje uzoraka poruka korporaciji Microsoft.</span><span class="sxs-lookup"><span data-stu-id="55004-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
