---
title: Prijavljivanje u Windows 10 bez upotrebe lozinke
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719967"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="5a201-102">Prijavljivanje u Windows 10 bez upotrebe lozinke</span><span class="sxs-lookup"><span data-stu-id="5a201-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="5a201-103">Da biste izbegli da otkucate lozinku na Windows pokretanju, preporučujemo vam da koristite neku od Windows Helo bezbednih opcija za prijavljivanje, kao što je PIN, prepoznavanje lica ili otisak prsta, ako je dostupno.</span><span class="sxs-lookup"><span data-stu-id="5a201-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="5a201-104">Ako zaista želite da onemogućite bezbedno prijavljivanje, pogledajte uputstva "automatski prijavljivanje u Windows 10".</span><span class="sxs-lookup"><span data-stu-id="5a201-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="5a201-105">**Bezbedni Windows Helo alternative lozinci za nalog**</span><span class="sxs-lookup"><span data-stu-id="5a201-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="5a201-106">**Izaberite stavke postavke > nalozima > opcijama za prijavljivanje** (ili kliknite [ovde](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="5a201-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="5a201-107">Dostupne opcije za prijavljivanje će biti navedene.</span><span class="sxs-lookup"><span data-stu-id="5a201-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="5a201-108">Na primer:</span><span class="sxs-lookup"><span data-stu-id="5a201-108">For example:</span></span>

![Opcije prijavljivanja.](media/sign-in-options.png)

<span data-ttu-id="5a201-110">Kliknite na neku od opcija da biste je konfigurisali.</span><span class="sxs-lookup"><span data-stu-id="5a201-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="5a201-111">Sledeći put kada pokrenete ili otključate Windows, moći ćete da koristite novu opciju umesto lozinke.</span><span class="sxs-lookup"><span data-stu-id="5a201-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="5a201-112">**Automatski prijavljivanje u Windows 10**</span><span class="sxs-lookup"><span data-stu-id="5a201-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="5a201-113">**Napomena**: automatsko prijavljivanje je zgodno, ali uvodi bezbednosni rizik, naročito ako je računaru pristupačan više osoba.</span><span class="sxs-lookup"><span data-stu-id="5a201-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="5a201-114">Kliknite ili dodirnite dugme **Start** na traci zadataka.</span><span class="sxs-lookup"><span data-stu-id="5a201-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="5a201-115">Otkucajte **netplwiz** i pritisnite taster ENTER da biste otvorili prozor korisnički nalozi.</span><span class="sxs-lookup"><span data-stu-id="5a201-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="5a201-116">U **korisničkim nalozima**izaberite nalog na koji želite da se automatski prijave kada se Windows pokrene.</span><span class="sxs-lookup"><span data-stu-id="5a201-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="5a201-117">Opozovite izbor u polju za potvrdu "korisnici moraju da unesu korisničko ime i lozinku da bi koristili ovaj računar".</span><span class="sxs-lookup"><span data-stu-id="5a201-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Korisnici moraju da unesu opciju korisničkog imena i lozinke.](media/users-must-enter-username.png)

5. <span data-ttu-id="5a201-119">Kliknite na dugme **U redu**.</span><span class="sxs-lookup"><span data-stu-id="5a201-119">Click **OK**.</span></span> <span data-ttu-id="5a201-120">Od vas će se tražiti da unesete i potvrdite lozinku za izabrani nalog.</span><span class="sxs-lookup"><span data-stu-id="5a201-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="5a201-121">Kliknite na dugme **u redu** da biste završili.</span><span class="sxs-lookup"><span data-stu-id="5a201-121">Click **OK** to finish.</span></span> <span data-ttu-id="5a201-122">Kada se Windows 10 pokrene, on će se automatski prijaviti na nalog koji ste izabrali.</span><span class="sxs-lookup"><span data-stu-id="5a201-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
