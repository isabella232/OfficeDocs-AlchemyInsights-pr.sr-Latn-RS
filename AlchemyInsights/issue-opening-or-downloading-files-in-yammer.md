---
title: Izdavanje ili preuzimanje datoteka na mreži Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148339"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="07593-102">Izdavanje ili preuzimanje datoteka na mreži Yammer</span><span class="sxs-lookup"><span data-stu-id="07593-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="07593-103">Classic Yammer podržava više opcija za otpremanje datoteka u poruke i grupe.</span><span class="sxs-lookup"><span data-stu-id="07593-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="07593-104">U zavisnosti od mrežne konfiguracije, datoteke koje se podrazumevano skladište u sistemu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="07593-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="07593-105">Birač datoteka na novoj mreži Yammer još uvek ne podržava sve opcije dostupne u klasičnom mreži Yammer.</span><span class="sxs-lookup"><span data-stu-id="07593-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="07593-106">Buduća ispravka će dodati dodatne funkcije.</span><span class="sxs-lookup"><span data-stu-id="07593-106">A future update will add additional features.</span></span> <span data-ttu-id="07593-107">Više informacija potražite u članku [Prilaganje datoteke ili slike na poruku razgovora o mreži Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="07593-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="07593-108">**Nije moguće otvoriti ili preuzeti datoteku**</span><span class="sxs-lookup"><span data-stu-id="07593-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="07593-109">Datoteka može da se otpremi na Yammer, ali se takođe povezuje sa datotekom na SharePoint mreži.</span><span class="sxs-lookup"><span data-stu-id="07593-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="07593-110">Prvo morate da utvrdite lokaciju datoteke da biste rešili problem.</span><span class="sxs-lookup"><span data-stu-id="07593-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="07593-111">Ako je datoteka otpremljena na Yammer, ona će imati \*. yammer.com URL.</span><span class="sxs-lookup"><span data-stu-id="07593-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="07593-112">Uverite se da su zahtevane URL adrese i IP adrese deblokirale.</span><span class="sxs-lookup"><span data-stu-id="07593-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="07593-113">Više informacija potražite u objavi bloga [koristeći čvrste šifrirane IP adrese za Yammer se ne preporučuje](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="07593-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="07593-114">Proverite da li je korisnik koji ujedno i globalni administrator može da preuzme datoteku.</span><span class="sxs-lookup"><span data-stu-id="07593-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="07593-115">Ako je datoteka privatna, možda ćete morati da koristite režim "privatan sadržaj".</span><span class="sxs-lookup"><span data-stu-id="07593-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="07593-116">Više informacija potražite [u članku nadgledanje privatnog sadržaja na mreži Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="07593-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="07593-117">**Gosti i datoteke na nivou mreže na mreži Yammer na SharePoint mreži**</span><span class="sxs-lookup"><span data-stu-id="07593-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="07593-118">[Gosti na mrežnom nivou na mreži Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne koriste "AZURE AD B2B" i interni su za uslugu Yammer, tako da ne mogu da pristupe datotekama Yammer uskladištenim u sistemu SharePoint.</span><span class="sxs-lookup"><span data-stu-id="07593-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="07593-119">Kreirajte eksterni AAD B2B korisnik koji može da pristupi bibliotekama dokumenata na SharePoint mreži koristeći taj identitet.</span><span class="sxs-lookup"><span data-stu-id="07593-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="07593-120">Za informacije o budućem Azure podršci za goste na mreži Yammer, podrška za goste na mreži za [poslovne korisnike (B2B) u usluzi Yammer Preview-uslovi i najčešća pitanja](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="07593-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>