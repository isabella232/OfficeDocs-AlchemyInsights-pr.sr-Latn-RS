---
title: Teams dozvoljavaju ili onemogućava IP video zapis
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826357"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="d7602-102">Teams dozvoljavaju ili onemogućava IP video zapis</span><span class="sxs-lookup"><span data-stu-id="d7602-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="d7602-103">**Promena ili kreiranje smernica za sastanak**</span><span class="sxs-lookup"><span data-stu-id="d7602-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="d7602-104">Da biste promenili ili kreirali smernice za sastanke, idite u **Microsoft Teams centar > "Sastanci> smernice za sastanke.**</span><span class="sxs-lookup"><span data-stu-id="d7602-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="d7602-105">Izaberite smernice sa liste ili kliknite na dugme **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="d7602-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="d7602-106">Ako pravite nove smernice, dodajte ime i opis.</span><span class="sxs-lookup"><span data-stu-id="d7602-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="d7602-107">Ime ne može da sadrži specijalne znakove ni da bude duže od 64 znaka.</span><span class="sxs-lookup"><span data-stu-id="d7602-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="d7602-108">Odaberite postavke i kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="d7602-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="d7602-109">Na primer, recimo da imate mnogo korisnika i želite da ograničite količinu propusnog propusnog ograničenja koji bi njihov sastanak zahtevao.</span><span class="sxs-lookup"><span data-stu-id="d7602-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="d7602-110">Napravićete nove prilagođene smernice pod imenom „Ograničeni propusni opseg“ i onemogućiti sledeće postavke:</span><span class="sxs-lookup"><span data-stu-id="d7602-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="d7602-111">U okviru **Audio i video**:</span><span class="sxs-lookup"><span data-stu-id="d7602-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="d7602-112">Isključite opciju „Dozvoli snimanje u oblaku“.</span><span class="sxs-lookup"><span data-stu-id="d7602-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="d7602-113">Isključite opciju „Dozvoli IP video“.</span><span class="sxs-lookup"><span data-stu-id="d7602-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="d7602-114">Zatim dodelite smernice korisnicima.</span><span class="sxs-lookup"><span data-stu-id="d7602-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="d7602-115">**Dodeljivanje smernica za sastanke korisnicima**</span><span class="sxs-lookup"><span data-stu-id="d7602-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="d7602-116">U levom okviru za navigaciju u Microsoft Teams centru administracije izaberite stavku **Korisnici** i kliknite na korisnika.</span><span class="sxs-lookup"><span data-stu-id="d7602-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="d7602-117">Izaberite korisnika tako što ćete kliknuti sa leve strane korisničkog imena, a zatim izaberite stavku **Uredi postavke**.</span><span class="sxs-lookup"><span data-stu-id="d7602-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="d7602-118">U **okviru Smernice za** sastanke izaberite smernice koje želite da dodelite, a zatim kliknite na **dugme Primeni**.</span><span class="sxs-lookup"><span data-stu-id="d7602-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="d7602-119">Dodatne informacije potražite u [temi Upravljanje smernicama za sastanke u timovima.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="d7602-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
