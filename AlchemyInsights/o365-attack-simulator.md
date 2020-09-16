---
title: 2681 simulator napada u programu Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759233"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="ff9b0-102">Simulator napada u programu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ff9b0-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="ff9b0-103">Nedostaje vam simulator za napad?</span><span class="sxs-lookup"><span data-stu-id="ff9b0-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="ff9b0-104">Simulator napada zahteva **Office 365 napredni plan zaštite od pretnje 2 (ATP plan 2)** ili **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="ff9b0-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="ff9b0-105">Simulator napada **nije** uključen u Office 365 napredni plan zaštite od pretnje 1 (ATP plan 1), Office 365 Enterprise E3 ili bilo koje Microsoft 365 aplikacije za pretplate.</span><span class="sxs-lookup"><span data-stu-id="ff9b0-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="ff9b0-106">Nalog koji koristite za pokretanje simuliranih napada zahteva opšte dozvole globalnog administratora ili administratora bezbednosti i potvrdu identiteta sa više faktora (MFA).</span><span class="sxs-lookup"><span data-stu-id="ff9b0-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="ff9b0-107">Više informacija o zahtevima za simulator napada potražite u [ovom članku](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="ff9b0-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="ff9b0-108">Važne stvari koje treba znati **o** simulacijama za napad</span><span class="sxs-lookup"><span data-stu-id="ff9b0-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="ff9b0-109">Ako je omogućeno MFA za ciljni nalog i ako je lozinka ispravno pogodila, nalog se neće prikazati kao kompromitovan (drugi faktor potvrde identiteta će biti nepotpun).</span><span class="sxs-lookup"><span data-stu-id="ff9b0-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="ff9b0-110">Datoteka lozinki ne može biti veća od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="ff9b0-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="ff9b0-111">Koristite jednu lozinku po redu i dodajte praznu liniju (povratni tip) posle poslednje lozinke na listi.</span><span class="sxs-lookup"><span data-stu-id="ff9b0-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="ff9b0-112">Važne stvari koje treba znati o **phishing** Prilaganje Priloži:</span><span class="sxs-lookup"><span data-stu-id="ff9b0-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="ff9b0-113">Po dizajnu, ne možete da obezbedite prilagođenu vrednost za **URL adresu za phishing server za prijavljivanje**.</span><span class="sxs-lookup"><span data-stu-id="ff9b0-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="ff9b0-114">Ako primalac koristi [programski dodatak "Omogućavanje poruke izveštaja](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " da bi izvestio o grešci kao phishing, možda nećete primati obaveštenja (jer je ovo simulirani napad).</span><span class="sxs-lookup"><span data-stu-id="ff9b0-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="ff9b0-115">Izveštaji: kada se završi simulirani napad, možete da kliknete na dugme **Detalji napada** da biste videli izveštaj.</span><span class="sxs-lookup"><span data-stu-id="ff9b0-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="ff9b0-116">Detaljna uputstva i nove funkcije u simulatoru za napad potražite [u članku napad simulatora u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="ff9b0-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
