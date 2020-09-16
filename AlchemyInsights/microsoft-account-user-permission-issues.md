---
title: Rešavanje problema – korisnik nije pronađen u direktorijumu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725421"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ea811-102">Rešavanje problema – korisnik nije pronađen u direktorijumu</span><span class="sxs-lookup"><span data-stu-id="ea811-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ea811-103">Ako korisnici primaju poruku o grešci "nije moguće pronaći korisnika" u direktorijumu, pokušajte ponovo da pokušate gde je tip problema korisnik.</span><span class="sxs-lookup"><span data-stu-id="ea811-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ea811-104">Sledeći koraci mogu da se završe radi rešavanja problema.</span><span class="sxs-lookup"><span data-stu-id="ea811-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ea811-105">Uverite se da je nalog koji je prihvatio poziv e-pošte isti nalog koji se koristi za prijavljivanje kasnije.</span><span class="sxs-lookup"><span data-stu-id="ea811-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ea811-106">Uverite se da korisnik koristi isti nalog za prihvatanje pozivnice i prijavljivanje na sajt.</span><span class="sxs-lookup"><span data-stu-id="ea811-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ea811-107">Više informacija potražite u članku [Upravljanje pseudonimima za Microsoft nalog </a> radi upravljanja Microsoft 365 prijavljivanju](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ea811-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ea811-108">Potražite sve stranice u kojima korisnik prima grešku.</span><span class="sxs-lookup"><span data-stu-id="ea811-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ea811-109">Dodavanje "/_layouts/15/osoba Le.aspx/membersigrupid = 0" (unutar dvostrukog navoda) do kraja URL adrese lokacije.</span><span class="sxs-lookup"><span data-stu-id="ea811-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ea811-110">Primer: https://< "stutoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ea811-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ea811-111">Izaberite korisnika sa liste.</span><span class="sxs-lookup"><span data-stu-id="ea811-111">Select the user from the list.</span></span>

- <span data-ttu-id="ea811-112">Na traci izaberite stavku **Ukloni korisničke dozvole** .</span><span class="sxs-lookup"><span data-stu-id="ea811-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ea811-113">Dodajte korisnika i ponovo pošaljite poziv korisniku.</span><span class="sxs-lookup"><span data-stu-id="ea811-113">Add back the User and Resend the invite to the user.</span></span>

