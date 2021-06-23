---
title: Omogućavanje SMTP potvrde identiteta i rešavanja problema
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077665"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="beff5-102">Omogućavanje SMTP potvrde identiteta i rešavanja problema</span><span class="sxs-lookup"><span data-stu-id="beff5-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="beff5-103">Ako želite da omogućite SMTP potvrdu identiteta za poštansko sanduče ili dobijate "Klijent nije ovlašten", Greška "Potvrda identiteta bezuspešno" ili "SmtpClientAuthentication" sa kodom 5.7.57 ili 5.7.3 ili 5.7.139 kada pokušate da pošaljete e-poštu potvrdom identiteta uređaja ili aplikacije pomoću usluge Microsoft 365, izvršite ove tri radnje da biste rešili problem:</span><span class="sxs-lookup"><span data-stu-id="beff5-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="beff5-104">Onemogućite [podrazumevane vrednosti bezbednosti za Azure](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) tako što će na vrednost "Omogući **podrazumevane vrednosti bezbednosti" onemogućiti** **vrednost "Ne"**.</span><span class="sxs-lookup"><span data-stu-id="beff5-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="beff5-105">a.</span><span class="sxs-lookup"><span data-stu-id="beff5-105">a.</span></span> <span data-ttu-id="beff5-106">Prijavite se na Azure portal kao administrator za bezbednost, administrator uslovnog pristupa ili globalni administrator.</span><span class="sxs-lookup"><span data-stu-id="beff5-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="beff5-107">b.</span><span class="sxs-lookup"><span data-stu-id="beff5-107">b.</span></span> <span data-ttu-id="beff5-108">Potražite svojstva  **Azure Active Directory >.**</span><span class="sxs-lookup"><span data-stu-id="beff5-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="beff5-109">c.</span><span class="sxs-lookup"><span data-stu-id="beff5-109">c.</span></span> <span data-ttu-id="beff5-110">Izaberite **stavku Upravljanje podrazumevanim vrednostima bezbednosti**.</span><span class="sxs-lookup"><span data-stu-id="beff5-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="beff5-111">d.</span><span class="sxs-lookup"><span data-stu-id="beff5-111">d.</span></span> <span data-ttu-id="beff5-112">Postavite **opciju Omogući podrazumevane vrednosti bezbednosti** na **Ne**.</span><span class="sxs-lookup"><span data-stu-id="beff5-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="beff5-113">e.</span><span class="sxs-lookup"><span data-stu-id="beff5-113">e.</span></span> <span data-ttu-id="beff5-114">Izaberite **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="beff5-114">Select **Save**.</span></span>

2. <span data-ttu-id="beff5-115">[Omogućite SMTP prosleđivanje klijenta](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) u licenciranom poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="beff5-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="beff5-116">a.</span><span class="sxs-lookup"><span data-stu-id="beff5-116">a.</span></span> <span data-ttu-id="beff5-117">Na Microsoft 365 centar administracije stavku **Aktivni** korisnici i izaberite korisnika.</span><span class="sxs-lookup"><span data-stu-id="beff5-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="beff5-118">b.</span><span class="sxs-lookup"><span data-stu-id="beff5-118">b.</span></span> <span data-ttu-id="beff5-119">Idite na karticu Pošta i u okviru **Aplikacije za e-poštu** izaberite stavku **Upravljanje aplikacijama za e-poštu**.</span><span class="sxs-lookup"><span data-stu-id="beff5-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="beff5-120">d.</span><span class="sxs-lookup"><span data-stu-id="beff5-120">d.</span></span> <span data-ttu-id="beff5-121">Proverite da li je potvrđena potvrda identiteta **SMTP** (omogućeno).</span><span class="sxs-lookup"><span data-stu-id="beff5-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="beff5-122">e.</span><span class="sxs-lookup"><span data-stu-id="beff5-122">e.</span></span> <span data-ttu-id="beff5-123">Izaberite **Sačuvaj promene**.</span><span class="sxs-lookup"><span data-stu-id="beff5-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="beff5-124">[Onemogućite uslugu Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) na licenciranom poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="beff5-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="beff5-125">a.</span><span class="sxs-lookup"><span data-stu-id="beff5-125">a.</span></span> <span data-ttu-id="beff5-126">Idite na prozor Microsoft 365 centar administracije u meniju navigacije sa leve strane izaberite stavku **Korisnici**  >  **aktivni korisnici.**</span><span class="sxs-lookup"><span data-stu-id="beff5-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="beff5-127">b.</span><span class="sxs-lookup"><span data-stu-id="beff5-127">b.</span></span> <span data-ttu-id="beff5-128">Izaberite **stavku Multi-Factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="beff5-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="beff5-129">c.</span><span class="sxs-lookup"><span data-stu-id="beff5-129">c.</span></span> <span data-ttu-id="beff5-130">Izaberite korisnika i **onemogućite Multi-Factor Auth**.</span><span class="sxs-lookup"><span data-stu-id="beff5-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
