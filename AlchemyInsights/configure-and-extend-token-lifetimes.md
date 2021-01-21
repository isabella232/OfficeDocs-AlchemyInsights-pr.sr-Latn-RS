---
title: Konfigurisanje i proširivanje simbola ћivotnih vekova
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917010"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="64280-102">Konfigurisanje i proširivanje simbola ћivotnih vekova</span><span class="sxs-lookup"><span data-stu-id="64280-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="64280-103">Možete da precizirate životni vek Access, SEMLA ili Token ID-a koji izdaje Microsoft platforma za identifikaciju.</span><span class="sxs-lookup"><span data-stu-id="64280-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="64280-104">Možete da postavljate Token ћivotna za sve aplikacije u organizaciji, za aplikaciju za više stanara (multi-organizacija) ili za određenu uslugu usluge u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="64280-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="64280-105">Da biste dobili više informacija, pročitajte simbol za čitanje u [čitljivom](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)programu.</span><span class="sxs-lookup"><span data-stu-id="64280-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="64280-106">Primere pročitajte [Kako da konfigurišete Token ћivota](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="64280-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="64280-107">Da biste saznali kako da konfigurišete trajanje i kompatibilnost simbola u članku Azure Active Directory B2C (Azure AD B2C), pogledajte članak [Konfigurisanje simbola u usluzi Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="64280-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="64280-108">Članak [konfiguriše ponašanje sesije u usluzi Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) opisuje metode za jedinstveno prijavljivanje (SSO) metodi koje se koriste u usluzi AZURE AD B2C i pomaže vam da odaberete NAJPRIKLADNIJI SSO metod prilikom konfigurisanja smernica.</span><span class="sxs-lookup"><span data-stu-id="64280-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="64280-109">**Koliko vremena traju? Koliko dugo traju?**</span><span class="sxs-lookup"><span data-stu-id="64280-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="64280-110">Token doћivotno je 1 sat i trajanje sesije je 24 časa.</span><span class="sxs-lookup"><span data-stu-id="64280-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="64280-111">To znači da ako nije bilo zahteva za 24 časa, moraćete ponovo da se prijavite pre nego što zatražite novi simbol.</span><span class="sxs-lookup"><span data-stu-id="64280-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="64280-112">Posle 30 maja 2020, nijedan novi zakupac neće moći da koristi polisu životnog simbola za konfiguraciju za konfigurisanje sesije i osvežavanje simbola.</span><span class="sxs-lookup"><span data-stu-id="64280-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="64280-113">Deprekacija će se desiti nekoliko meseci posle toga, što znači da ćemo prestati da poštićemo postojeće sesije i osvežavamo polise tikena.</span><span class="sxs-lookup"><span data-stu-id="64280-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="64280-114">I dalje možete da konfigurišete oznaku za pristup ћivotna posle deprekacije.</span><span class="sxs-lookup"><span data-stu-id="64280-114">You can still configure access token lifetimes after the deprecation.</span></span>






