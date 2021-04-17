---
title: Prijavljivanje u Windows 10 bez korišćenja lozinke
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830560"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="bc788-102">Prijavljivanje u Windows 10 bez korišćenja lozinke</span><span class="sxs-lookup"><span data-stu-id="bc788-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="bc788-103">Da biste izbegli da morate da otkucate lozinku pri pokretanju operativnog sistema Windows, preporučujemo da koristite jednu od opcija za bezbedno prijavljivanje na Windows Hello, kao što je PIN, prepoznavanje lica ili otisak prsta, ako je dostupna.</span><span class="sxs-lookup"><span data-stu-id="bc788-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="bc788-104">Ako zaista želite da onemogućite bezbedno prijavljivanje, pogledajte uputstva "Automatsko prijavljivanje u Windows 10" u nastavku.</span><span class="sxs-lookup"><span data-stu-id="bc788-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="bc788-105">**Zaštita Windows Hello alternativa za lozinku naloga**</span><span class="sxs-lookup"><span data-stu-id="bc788-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="bc788-106">Izaberite **stavke Postavke > naloge > za prijavljivanje** (ili kliknite [ovde](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="bc788-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="bc788-107">Navodi se dostupne opcije za prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="bc788-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="bc788-108">Na primer:</span><span class="sxs-lookup"><span data-stu-id="bc788-108">For example:</span></span>

![Opcije za prijavljivanje.](media/sign-in-options.png)

<span data-ttu-id="bc788-110">Kliknite na jednu od opcija ili je dodirnite da biste je konfigurisali.</span><span class="sxs-lookup"><span data-stu-id="bc788-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="bc788-111">Sledeći put kada pokrenete ili otključate Windows, moći ćete da koristite novu opciju umesto lozinke.</span><span class="sxs-lookup"><span data-stu-id="bc788-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="bc788-112">**Automatsko prijavljivanje u Windows 10**</span><span class="sxs-lookup"><span data-stu-id="bc788-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="bc788-113">**Naznaka:** Automatsko prijavljivanje je praktično, ali predstavlja bezbednosni rizik, naročito ako računaru može da pristupi više osoba.</span><span class="sxs-lookup"><span data-stu-id="bc788-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="bc788-114">Kliknite na dugme **Start ili ga** dodirnite na traci zadataka.</span><span class="sxs-lookup"><span data-stu-id="bc788-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="bc788-115">Otkucajte **netplwiz i** kliknite na taster Enter da biste otvorili prozor "Korisnički nalozi".</span><span class="sxs-lookup"><span data-stu-id="bc788-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="bc788-116">U **dijalozima Korisnički** nalozi izaberite nalog na koji želite da se automatski prijavite kada se Windows pokrene.</span><span class="sxs-lookup"><span data-stu-id="bc788-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="bc788-117">Poništite izbor u polju za potvrdu "Korisnici moraju da uneli korisničko ime i lozinku da bi koristili ovaj računar".</span><span class="sxs-lookup"><span data-stu-id="bc788-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Korisnici moraju uneti opciju korisničkog imena i lozinke.](media/users-must-enter-username.png)

5. <span data-ttu-id="bc788-119">Kliknite na dugme **U redu**.</span><span class="sxs-lookup"><span data-stu-id="bc788-119">Click **OK**.</span></span> <span data-ttu-id="bc788-120">Bićete upitani da unesete i potvrdite lozinku za nalog koji ste izabrali.</span><span class="sxs-lookup"><span data-stu-id="bc788-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="bc788-121">Kliknite na **dugme U redu** da biste završili.</span><span class="sxs-lookup"><span data-stu-id="bc788-121">Click **OK** to finish.</span></span> <span data-ttu-id="bc788-122">Sledeći put kada se Windows 10 pokrene, on će se automatski prijaviti na nalog koji ste izabrali.</span><span class="sxs-lookup"><span data-stu-id="bc788-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
