---
title: Korisnik prima grešku AADSTS7000112 Yammer je onemogućen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198373"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="fbd29-102">Korisnik prima grešku AADSTS7000112 Yammer je onemogućen</span><span class="sxs-lookup"><span data-stu-id="fbd29-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="fbd29-103">Ako dobijete poruku o pogrešci "AADSTS7000112: Application ' 00000005-0000-0ff1-CE00-000000000000" (Yammer) je onemogućen ", postoji problem sa direktorom usluge u okviru" Azure oglasa ".</span><span class="sxs-lookup"><span data-stu-id="fbd29-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="fbd29-104">Administrator je možda onemogućio direktora usluge da bi blokirao pristup mreži Yammer.</span><span class="sxs-lookup"><span data-stu-id="fbd29-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="fbd29-105">Onemogućavanje glavnice usluge se ne preporučuje i može izazvati dodatne probleme.</span><span class="sxs-lookup"><span data-stu-id="fbd29-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="fbd29-106">Više informacija o podržanom pristupu za blokiranje korisničkog pristupa Yammer potražite [u članku isključivanje pristupa na mreži za korisnike kompanije Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="fbd29-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="fbd29-107">Da biste otklonili ovaj problem na Azure portalu i vratili korisnički pristup na Yammer:</span><span class="sxs-lookup"><span data-stu-id="fbd29-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="fbd29-108">Otvorite stranicu "Azure Active Directory" i izaberite **poslovne aplikacije** u okviru stavke " **Upravljanje** " u levom oknu za navigaciju.</span><span class="sxs-lookup"><span data-stu-id="fbd29-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="fbd29-109">U polje za pretragu otkucajte **Office 365 Yammer** , a zatim izaberite ime aplikacije da biste otvorili postavke.</span><span class="sxs-lookup"><span data-stu-id="fbd29-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="fbd29-110">Izaberite **Svojstva** u okviru " **Upravljanje** " u levom oknu za navigaciju.</span><span class="sxs-lookup"><span data-stu-id="fbd29-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="fbd29-111">Podesite vrednost **omogućenog za korisnike da se prijave?** na **da**, a zatim kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="fbd29-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="fbd29-112">Ponovo se prijavite na Yammer.</span><span class="sxs-lookup"><span data-stu-id="fbd29-112">Sign in to Yammer again.</span></span> <span data-ttu-id="fbd29-113">Možda će biti potrebno da obrišete kolačiće.</span><span class="sxs-lookup"><span data-stu-id="fbd29-113">You might need to clear cookies.</span></span>

<span data-ttu-id="fbd29-114">Druga mogućnost je da pokrenete komande PowerShell da biste postavili vrednost.</span><span class="sxs-lookup"><span data-stu-id="fbd29-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="fbd29-115">Za više informacija, pogledajte ["Izvini, ali imamo problema sa prijavljivanjem" kada kliknete na pločicu "Yammer" u sistemu Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="fbd29-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 