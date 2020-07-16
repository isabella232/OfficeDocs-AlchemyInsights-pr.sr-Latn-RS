---
title: Rešavanje problema sa učitavanjem slika na mreži Yammer
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
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148297"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="ccaff-102">Rešavanje problema sa učitavanjem slika na mreži Yammer</span><span class="sxs-lookup"><span data-stu-id="ccaff-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="ccaff-103">Kada se problemi javljaju sa fotografijama i pregledima datoteka u mreži Yammer, rešite problem tako što ćete proveriti da li se problem javlja za sve korisnike, bez obzira na to da li se on pojavljuje na mobilnim uređajima i ako je moguće ponovo produktivno prilikom otpremanja priloga.</span><span class="sxs-lookup"><span data-stu-id="ccaff-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="ccaff-104">**Problemi sa fotografijama profila**</span><span class="sxs-lookup"><span data-stu-id="ccaff-104">**Profile photo issues**</span></span>  

<span data-ttu-id="ccaff-105">Ako se krajnji korisnici prijave na Yammer preko Microsoft 365, moraju da promene svoj profil, uključujući i fotografiju profila.</span><span class="sxs-lookup"><span data-stu-id="ccaff-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="ccaff-106">Ako korisnicima nije dozvoljeno da naprave ispravke profila, administrator može da napravi ispravku za korisnika.</span><span class="sxs-lookup"><span data-stu-id="ccaff-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="ccaff-107">Više informacija potražite u članku [prikaz i ažuriranje profila u sistemu Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="ccaff-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="ccaff-108">Informacije o uređivanju profila, uključujući fotografije profila, potražite u članku [Promena profila i postavki za Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="ccaff-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="ccaff-109">Ažurirane fotografije profila su sinhronizovane drugačije od atributa profila.</span><span class="sxs-lookup"><span data-stu-id="ccaff-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="ccaff-110">Korisnici moraju da se prijave da bi pokrenuli sinhronizaciju svoje fotografije profila.</span><span class="sxs-lookup"><span data-stu-id="ccaff-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="ccaff-111">Više informacija potražite u članku [slike korisničkog profila ažurirane sa Office 365 na Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="ccaff-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="ccaff-112">Za informacije o korisničkom životnom ciklusu za Yammer pogledajte odeljak [Upravljanje korisnicima mreže Yammer preko njihovog životnog ciklusa iz sistema Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="ccaff-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="ccaff-113">Detalje o tome kako sinhronizacija slike profila funkcioniše u programu Microsoft 365 potražite u članku [informacije o sinhronizaciji slike profila u programu microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="ccaff-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="ccaff-114">**Problemi sa pregledima i sličicama slika**</span><span class="sxs-lookup"><span data-stu-id="ccaff-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="ccaff-115">Kada se datoteke ili slike knjiže na Yammer, pregledi se možda neće pojaviti zato što:</span><span class="sxs-lookup"><span data-stu-id="ccaff-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="ccaff-116">Datoteka je oštećena i ne može se obraditi.</span><span class="sxs-lookup"><span data-stu-id="ccaff-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="ccaff-117">Datoteka nije nedavno otpremljena u SharePoint Online ili Yammer ima nevažeće metapodatke iz drugih razloga.</span><span class="sxs-lookup"><span data-stu-id="ccaff-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="ccaff-118">URL adrese potrebne za učitavanje slika za pregled su blokirane.</span><span class="sxs-lookup"><span data-stu-id="ccaff-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="ccaff-119">Korisnik je uklonio pregled datoteka pre knjiženja.</span><span class="sxs-lookup"><span data-stu-id="ccaff-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="ccaff-120">Problem usluge je sprečio da se generiše pregled.</span><span class="sxs-lookup"><span data-stu-id="ccaff-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="ccaff-121">**Belešku** Pregledi za veze i otpremanje datoteka mogu da se ponašaju drugačije.</span><span class="sxs-lookup"><span data-stu-id="ccaff-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="ccaff-122">Veze ka datotekama na Internetu ili vezama koje zahtevaju dodatnu potvrdu identiteta možda neće biti ispravno prikazane.</span><span class="sxs-lookup"><span data-stu-id="ccaff-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="ccaff-123">Više informacija potražite u članku [Prilaganje datoteke ili slike u poruku Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="ccaff-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 