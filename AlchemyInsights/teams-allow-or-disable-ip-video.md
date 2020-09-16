---
title: Timovi omogućite ili onemogućite IP video
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670198"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="ae3a6-102">Timovi omogućite ili onemogućite IP video</span><span class="sxs-lookup"><span data-stu-id="ae3a6-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="ae3a6-103">**Promena ili kreiranje smernica za sastanak**</span><span class="sxs-lookup"><span data-stu-id="ae3a6-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="ae3a6-104">Da biste promenili ili kreirali smernice sastanka, idite u **Microsoft centar administracije > sastanci > smernicama za sastanke**.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="ae3a6-105">Izaberite smernice sa liste ili kliknite na dugme **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="ae3a6-106">Ako pravite nove smernice, dodajte ime i opis.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="ae3a6-107">Ime ne može da sadrži specijalne znakove ni da bude duže od 64 znaka.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="ae3a6-108">Odaberite postavke i kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="ae3a6-109">Na primer, recimo da imate mnogo korisnika i želite da ograničite količinu propusnog opsega koji će im biti potreban.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="ae3a6-110">Napravićete nove prilagođene smernice pod imenom „Ograničeni propusni opseg“ i onemogućiti sledeće postavke:</span><span class="sxs-lookup"><span data-stu-id="ae3a6-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="ae3a6-111">U okviru **Audio i video**:</span><span class="sxs-lookup"><span data-stu-id="ae3a6-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="ae3a6-112">Isključite opciju „Dozvoli snimanje u oblaku“.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="ae3a6-113">Isključite opciju „Dozvoli IP video“.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="ae3a6-114">Zatim dodelite smernice korisnicima.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="ae3a6-115">**Dodeljivanje smernica za sastanke korisnicima**</span><span class="sxs-lookup"><span data-stu-id="ae3a6-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="ae3a6-116">U levom okviru za navigaciju u Microsoft Teams centru administracije izaberite stavku **Korisnici** i kliknite na korisnika.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="ae3a6-117">Izaberite korisnika tako što ćete kliknuti sa leve strane korisničkog imena, a zatim izaberite stavku **Uredi postavke**.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="ae3a6-118">U okviru **smernice za sastanak**izaberite smernice koje želite da dodelite, a zatim kliknite na dugme **Prijavi**se.</span><span class="sxs-lookup"><span data-stu-id="ae3a6-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="ae3a6-119">Više informacija potražite u članku [Upravljanje smernicama za sastanke u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ae3a6-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
