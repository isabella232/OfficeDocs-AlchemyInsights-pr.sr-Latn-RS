---
title: Problemi sa licenkom Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657290"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="f37d6-102">Problemi sa licenkom Yammer</span><span class="sxs-lookup"><span data-stu-id="f37d6-102">Yammer licensing issues</span></span>

<span data-ttu-id="f37d6-103">Svi korisnici moraju da imaju licencu za korišćenje usluge Yammer Enterprise, ali podrazumevano Yammer ne zahteva da korisnici imaju licencu za pristup usluzi.</span><span class="sxs-lookup"><span data-stu-id="f37d6-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="f37d6-104">Kada administrator promeni postavku tako da blokira Microsoft 365 korisnike bez Yammer licenci, korisnici koji nemaju Yammer Enterprise licencu ne mogu da pristupe Yammer usluzi.</span><span class="sxs-lookup"><span data-stu-id="f37d6-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="f37d6-105">Više informacija potražite u članku [Upravljanje korisničkim licencama usluge Yammer u sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="f37d6-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="f37d6-106">Kada se licence uklone sa korisnika, pločica Yammer više se ne prikazuje, a druge usluge mogu da koriste uklanjanje licenci za skrivanje funkcija.</span><span class="sxs-lookup"><span data-stu-id="f37d6-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="f37d6-107">U drugim slučajevima, funkcije se i dalje mogu pojavljivati, ali zahtevaju da se zadatak licence radi.</span><span class="sxs-lookup"><span data-stu-id="f37d6-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="f37d6-108">**Licenca se ne ažurira za korisnika**</span><span class="sxs-lookup"><span data-stu-id="f37d6-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="f37d6-109">Povremeno je korisniku dodeljena licenca, ali još uvek ne može da pristupi Yammeru.</span><span class="sxs-lookup"><span data-stu-id="f37d6-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="f37d6-110">Kašnjenje se može pojaviti kada je u toku dodela masovne licence.</span><span class="sxs-lookup"><span data-stu-id="f37d6-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="f37d6-111">Yammer korisnici se možda neće ažurirati istim redosledom kao što se licence menjaju u usluzi Azure AD zato što se sistem asinhrono pokreće.</span><span class="sxs-lookup"><span data-stu-id="f37d6-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="f37d6-112">Sačekajte 24 časa pre otvaranja slučaja podrške da biste prijavili probleme sa sinhronizacijom licence.</span><span class="sxs-lookup"><span data-stu-id="f37d6-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="f37d6-113">**Dodela masovne licence**</span><span class="sxs-lookup"><span data-stu-id="f37d6-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="f37d6-114">Licence se mogu dodeliti administratorskom centru ili PowerShell Scripting.</span><span class="sxs-lookup"><span data-stu-id="f37d6-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="f37d6-115">Više informacija potražite u članku [dodeljivanje licenci korisnicima](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [dodeljivanje licenci korisničkim nalozima pomoću usluge Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="f37d6-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="f37d6-116">Microsoft podrška ne pruža pomoć za kreiranje skripti, ali je dostupna dokumentacija za Yammer zadatak licence.</span><span class="sxs-lookup"><span data-stu-id="f37d6-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="f37d6-117">Više informacija potražite u članku [Upravljanje uslugom Yammer pomoću programa Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="f37d6-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>