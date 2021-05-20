---
title: Poruka "Nije pronađena nijedna pretplata" u centru za bezbednost
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
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544122"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="4f170-102">Poruka "Nije pronađena nijedna pretplata" u centru za bezbednost</span><span class="sxs-lookup"><span data-stu-id="4f170-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="4f170-103">Ako prilikom pristupa programu Centar za bezbednost Microsoft zaštitnika dobijete poruku "Pretplata nije pronađena", to znači da Azure Active Directory (AAD) koji se koristi za prijavljivanje korisnika na portal nema licencu za ATP za Microsoft zaštitnik.</span><span class="sxs-lookup"><span data-stu-id="4f170-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="4f170-104">Licence za Windows E5 i Kancelarija E5 su odvojene licence.</span><span class="sxs-lookup"><span data-stu-id="4f170-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="4f170-105">Otvorite predmet podrške ako je licenca kupena, ali nije obezbeđena za ovu AAD instancu.</span><span class="sxs-lookup"><span data-stu-id="4f170-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="4f170-106">Ili imate:</span><span class="sxs-lookup"><span data-stu-id="4f170-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="4f170-107">Mogući problem sa dodeljanjem licenci.</span><span class="sxs-lookup"><span data-stu-id="4f170-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="4f170-108">Nenamerno ste dodeljali licencu drugom Microsoft AAD-u od one koja se koristi za potvrdu identiteta u usluzi.</span><span class="sxs-lookup"><span data-stu-id="4f170-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>