---
title: Nije pronađena pretplata u centru bezbednosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713964"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="3ccaa-102">Nije pronađena pretplata u centru bezbednosti</span><span class="sxs-lookup"><span data-stu-id="3ccaa-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="3ccaa-103">Ako pri pristupu programu Security Center Microsoft Defender dobijete poruku "pronađena je nepretplata", to znači da je Azure Active Directory (AAD) korišćeno za prijavljivanje korisnika na portal nema ATP licence Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="3ccaa-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="3ccaa-104">Licence za Windows E5 i Office E5 su odvojene licence.</span><span class="sxs-lookup"><span data-stu-id="3ccaa-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="3ccaa-105">Otvorite slučaj podrške ako je licenca kupljena, ali nije dodeljena ovoj instanci.</span><span class="sxs-lookup"><span data-stu-id="3ccaa-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="3ccaa-106">Imate:</span><span class="sxs-lookup"><span data-stu-id="3ccaa-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="3ccaa-107">Mogući problem sa dozvolom licence.</span><span class="sxs-lookup"><span data-stu-id="3ccaa-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="3ccaa-108">Nenamerno ste snabdevali licencom različitom Microsoft AAD od one koja se koristi za potvrdu identiteta u usluzi.</span><span class="sxs-lookup"><span data-stu-id="3ccaa-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>