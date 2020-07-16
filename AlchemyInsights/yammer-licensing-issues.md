---
title: Problemi sa licenciranjem Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148319"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="6d84a-102">Problemi sa licenciranjem Yammer</span><span class="sxs-lookup"><span data-stu-id="6d84a-102">Yammer licensing issues</span></span>

<span data-ttu-id="6d84a-103">Svi korisnici moraju da imaju licencu za korišćenje usluge Yammer Enterprise, ali podrazumevano nije potrebno da korisnici imaju licencu za pristup usluzi.</span><span class="sxs-lookup"><span data-stu-id="6d84a-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="6d84a-104">Kada administrator promeni postavku za blokiranje Microsoft 365 korisnika bez licenci za Yammer, korisnici nisu dodelili licencu za Yammer Enterprise, ne mogu da pristupe usluzi Yammer.</span><span class="sxs-lookup"><span data-stu-id="6d84a-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="6d84a-105">Više informacija potražite u članku [Upravljanje korisničkim licencama za Yammer u sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="6d84a-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="6d84a-106">Kada se licence uklone od korisnika, pločica Yammer više nije prikazana, a druge usluge mogu da koriste uklanjanje licence za skrivanje funkcija.</span><span class="sxs-lookup"><span data-stu-id="6d84a-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="6d84a-107">U drugim slučajevima, funkcije se i dalje mogu pojaviti, ali zahtevaju dodelu dozvole za rad.</span><span class="sxs-lookup"><span data-stu-id="6d84a-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="6d84a-108">**Licenca se ne ažurira za korisnika**</span><span class="sxs-lookup"><span data-stu-id="6d84a-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="6d84a-109">Korisniku se povremeno dodeljuje licenca, ali i dalje ne može da pristupi mreži Yammer.</span><span class="sxs-lookup"><span data-stu-id="6d84a-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="6d84a-110">Verovatnije je da će doći do kašnjenja kada je dodela masovne dozvole u toku.</span><span class="sxs-lookup"><span data-stu-id="6d84a-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="6d84a-111">Korisnici mreže Yammer možda neće biti ažurirani u istom redosledu u kome se licence menjaju u Azure OGLASU jer se sistem asinhrono pokreće.</span><span class="sxs-lookup"><span data-stu-id="6d84a-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="6d84a-112">Sačekajte do 24 sata pre nego što otvorite predmet podrške da biste prijavili probleme sa sinhronizacijom licence.</span><span class="sxs-lookup"><span data-stu-id="6d84a-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="6d84a-113">**Dodeljivanje masovne dozvole**</span><span class="sxs-lookup"><span data-stu-id="6d84a-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="6d84a-114">Licence se mogu dodeliti putem administratorskog centra ili skriptovanja PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6d84a-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="6d84a-115">Više informacija potražite u članku [dodeljivanje licenci korisnicima](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [dodeljivanje licenci korisničkim nalozima pomoću sistema Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="6d84a-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="6d84a-116">Microsoft podrška ne pruža pomoć pri kreiranju skripti, ali je dostupna dokumentacija o dodeljnoj dodeli licenci za Yammer.</span><span class="sxs-lookup"><span data-stu-id="6d84a-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="6d84a-117">Više informacija potražite u članku [upravljanje licencama za Yammer pomoću Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="6d84a-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>