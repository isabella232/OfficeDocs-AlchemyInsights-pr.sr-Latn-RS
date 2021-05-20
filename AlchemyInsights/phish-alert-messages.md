---
title: 2491 Obaveštenje e-poruka od smernica "Phish Delivered due to tenant or user override"
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544592"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="fadae-102">Upozorenje e-poruka iz smernica "Phish Delivered due to zakupca ili user override"</span><span class="sxs-lookup"><span data-stu-id="fadae-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="fadae-103">Podrazumevane smernice za obaveštenja "Phish Delivered due to tenant or user override" dostavljaju se zakupcima koji imaju licence za Office 365 P1 i P2.</span><span class="sxs-lookup"><span data-stu-id="fadae-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="fadae-104">Ako ste dobili ovo obaveštenje, evo koraka koje treba da istražite:</span><span class="sxs-lookup"><span data-stu-id="fadae-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="fadae-105">U poruci upozorenja izaberite stavku  **Prikaži obaveštenje** da biste prešli na stranicu Obaveštenja u centru za & za usaglašenost.</span><span class="sxs-lookup"><span data-stu-id="fadae-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="fadae-106">Izaberite obaveštenje da biste videli opciju Prikaži **listu poruka ili Prikaži** poruke u **programu Explorer.**</span><span class="sxs-lookup"><span data-stu-id="fadae-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="fadae-107">Obe ove opcije će vas odvesti do detalja poruke koja sadrži ID poruke.</span><span class="sxs-lookup"><span data-stu-id="fadae-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="fadae-108">Imajte napom da će veza "Istraživač pretnji" automatski filtrirati poruke koje ispunjavaju kriterijume upozorenja.</span><span class="sxs-lookup"><span data-stu-id="fadae-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="fadae-109">Možda ćete morati da prilagodite filter datuma u programu Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="fadae-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="fadae-110">Phishing poruka je isporučena zbog ručno konfigurisane zamene:</span><span class="sxs-lookup"><span data-stu-id="fadae-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="fadae-111">Dozvoljeni pošiljalac ili domen koji je postavio korisnik.</span><span class="sxs-lookup"><span data-stu-id="fadae-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="fadae-112">Dozvoljenog pošiljaoca ili domena koje je postavio administratovani pošiljalac u smernicama za borbu protiv spam e-pošiljke.</span><span class="sxs-lookup"><span data-stu-id="fadae-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="fadae-113">Dozvoljena IP adresa u smernicama filtera veze.</span><span class="sxs-lookup"><span data-stu-id="fadae-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="fadae-114">Pravilo protoka pošte (poznato i kao pravilo za prenos) koje je konfigurisano tako da dozvoljava slanje poruka.</span><span class="sxs-lookup"><span data-stu-id="fadae-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="fadae-115">Ako smatrate da je poruka pogrešno označena kao phish, koristite programski dodatak Outlook [Report Message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) da biste prosledili uzorke poruka korporaciji Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fadae-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
