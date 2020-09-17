---
title: Vraćanje izbrisane datoteke ili fascikle u prethodno stanje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797562"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="a454a-102">Vraćanje izbrisane datoteke ili fascikle u prethodno stanje</span><span class="sxs-lookup"><span data-stu-id="a454a-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="a454a-103">SharePoint Online zadržava rezervne kopije celokupnog sadržaja još 14 dana nakon stvarnog brisanja.</span><span class="sxs-lookup"><span data-stu-id="a454a-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="a454a-104">Ako se sadržaj ne može vratiti kroz korpu za otpatke ili vraćanje datoteka u prethodno stanje, administrator može da se kontaktira sa Microsoft podrškom da bi zahtevao vraćanje u 14 dnevnom vremenu.</span><span class="sxs-lookup"><span data-stu-id="a454a-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="a454a-105">Vraćanja iz rezervnih kopija mogu da se obave samo za kolekcije sajtova ili podsajtove, ne i za pojedinačne datoteke, liste ili biblioteke.</span><span class="sxs-lookup"><span data-stu-id="a454a-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="a454a-106">Kada izbrišete stavku ili sajt iz sistema SharePoint, nije odmah uklonjena.</span><span class="sxs-lookup"><span data-stu-id="a454a-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="a454a-107">Izbrisane stavke idu u korpu za otpatke tokom određenog vremenskog perioda.</span><span class="sxs-lookup"><span data-stu-id="a454a-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="a454a-108">Tokom tog vremena stavke koje izbrisali možete da vratite na originalnu lokaciju.</span><span class="sxs-lookup"><span data-stu-id="a454a-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="a454a-109">Za više informacija posetite dolenavedene veze.</span><span class="sxs-lookup"><span data-stu-id="a454a-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="a454a-110">[Vraćanje stavki u korpu za otpatke SharePoint lokacije](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="a454a-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="a454a-111">Vraćanje izbrisanih datoteka ili fascikli u usluzi OneDrive</span><span class="sxs-lookup"><span data-stu-id="a454a-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="a454a-112">Vraćanje izbrisane kolekcije lokacija (uključujući grupu, komunikaciju i druge lokacije)</span><span class="sxs-lookup"><span data-stu-id="a454a-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="a454a-113">Vraćanje izbrisane OneDrive sajta u prethodno stanje</span><span class="sxs-lookup"><span data-stu-id="a454a-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="a454a-114">Za radnje korpe za masovno otpatke, administratori mogu da razmišljaju o korišćenju [sistema SharePoint online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="a454a-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="a454a-115">**Funkcija vraćanja datoteka u prethodno stanje**</span><span class="sxs-lookup"><span data-stu-id="a454a-115">**Files Restore feature**</span></span>

<span data-ttu-id="a454a-116">Ako se mnogo vaše OneDrive ili SharePoint datoteke brišu, prepišu, oštete ili zaražene malverom, možete da vratite celokupnu OneDrive ili SharePoint biblioteku na prethodno vreme pomoću funkcije Restore Restore datoteke.</span><span class="sxs-lookup"><span data-stu-id="a454a-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="a454a-117">Vraćanje OneDrive biblioteke</span><span class="sxs-lookup"><span data-stu-id="a454a-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="a454a-118">Vraćanje biblioteke dokumenata</span><span class="sxs-lookup"><span data-stu-id="a454a-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

