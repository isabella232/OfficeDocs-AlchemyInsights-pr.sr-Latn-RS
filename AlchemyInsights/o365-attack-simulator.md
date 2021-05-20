---
title: 2681 Simulator napada u Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545740"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="080b2-102">Simulator napada u Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="080b2-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="080b2-103">Da li vam nedostaje Simulator napada?</span><span class="sxs-lookup"><span data-stu-id="080b2-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="080b2-104">Simulator napada zahteva **Microsoft zaštitnik za Office 365 Plan 2** **ili Office 365 Enterprise E5.**</span><span class="sxs-lookup"><span data-stu-id="080b2-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="080b2-105">Simulator napada  nije uključen u Microsoft zaštitnik za Office 365 Plan 1, Office 365 Enterprise E3 ili bilo koje Microsoft 365 aplikacije za posao pretplate.</span><span class="sxs-lookup"><span data-stu-id="080b2-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="080b2-106">Nalog koji koristite za pokretanje simuliranih napada zahteva dozvole globalnog administratora ili administratora bezbednosti i višestruku potvrdu identiteta (MFA).</span><span class="sxs-lookup"><span data-stu-id="080b2-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="080b2-107">Više informacija o zahtevima simulatora napada potražite u [ovoj temi.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="080b2-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="080b2-108">Važne stvari koje treba znati o **simulacijama** napada brute i lozinke:</span><span class="sxs-lookup"><span data-stu-id="080b2-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="080b2-109">Ako ciljni nalog ima omogućen MFA, a lozinka je ispravno pogađana, nalog se neće prikazati kao ugrožen (drugi faktor za potvrdu identiteta će biti nedovršen).</span><span class="sxs-lookup"><span data-stu-id="080b2-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="080b2-110">Datoteka lozinke ne može biti veća od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="080b2-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="080b2-111">Koristite jednu lozinku po redu i unesite prazan red (povratak na red reda) posle poslednje lozinke na listi.</span><span class="sxs-lookup"><span data-stu-id="080b2-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="080b2-112">Važne stvari koje treba znati **o Spear phishingu** prilaže simulacije:</span><span class="sxs-lookup"><span data-stu-id="080b2-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="080b2-113">Po dizajnu, ne možete da obezbedite prilagođenu vrednost za **URL adresu servera** za prijavljivanje na Phishing.</span><span class="sxs-lookup"><span data-stu-id="080b2-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="080b2-114">Ako primalac koristi programski dodatak Omogući poruku izveštaja da prijavi poruku kao phishing, možda neće primiti obaveštenja za poruku (zato što je [to](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) simulirani napad).</span><span class="sxs-lookup"><span data-stu-id="080b2-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="080b2-115">Izveštaji: Kada se simulirani napad dovrši, možete da kliknete na dugme Detalji **o napadu** da biste videli izveštaj.</span><span class="sxs-lookup"><span data-stu-id="080b2-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="080b2-116">Detaljna uputstva i nove funkcije u simulatoru napada, pogledajte [Simulator](/microsoft-365/security/office-365-security/attack-simulator)napada u operativnom Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="080b2-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
