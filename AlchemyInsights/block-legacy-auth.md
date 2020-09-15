---
title: Blocklegalizacyauth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685612"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="bbce2-102">Blokiranje zastarele potvrde identiteta</span><span class="sxs-lookup"><span data-stu-id="bbce2-102">Blocking legacy authentication</span></span>

<span data-ttu-id="bbce2-103">Zastarela potvrda identiteta je termin koji se odnosi na zahtev za potvrdu identiteta koji je napravio:</span><span class="sxs-lookup"><span data-stu-id="bbce2-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="bbce2-104">Stariji Office klijenti koji ne koriste modernu potvrdu identiteta (na primer, Office 2010 klijent).</span><span class="sxs-lookup"><span data-stu-id="bbce2-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="bbce2-105">Bilo koji klijent koji koristi zastarele e-protokole kao što je IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="bbce2-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="bbce2-106">Više informacija o blokiranju zastarele potvrde identiteta i omogućavanju moderne potvrde identiteta potražite u okviru [blokiranje zastarele potvrde identiteta](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="bbce2-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="bbce2-107">Podrazumevane vrednosti bezbednosti u usluzi Azure Active Directory (Azure AD) olakšavaju bezbednost i zaštitu organizacije.</span><span class="sxs-lookup"><span data-stu-id="bbce2-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="bbce2-108">Podrazumevane vrednosti bezbednosti sadrže unapred podešene bezbednosne postavke za uobičajene napade.</span><span class="sxs-lookup"><span data-stu-id="bbce2-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="bbce2-109">Više informacija o podrazumevanim postavkama potražite u članku [Šta su to podrazumevane vrednosti bezbednosti?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="bbce2-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="bbce2-110">**Napomena**: ako je vaš zakupac kreiran na ili posle 22 oktobra, 2019, moguće je da nailazite na novo osigurano ponašanje i da već imate omogućene podrazumevane vrednosti za zakupca.</span><span class="sxs-lookup"><span data-stu-id="bbce2-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="bbce2-111">U pokušaju da zaštitite sve korisnike, podrazumevane vrednosti bezbednosti se udružu sa svim novim zakupcima kreiranim.</span><span class="sxs-lookup"><span data-stu-id="bbce2-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
