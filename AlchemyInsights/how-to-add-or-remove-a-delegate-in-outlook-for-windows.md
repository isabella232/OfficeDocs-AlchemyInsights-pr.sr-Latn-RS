---
title: Dodavanje ili uklanjanje delegata u programu Outlook za Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573572"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="946db-102">Dodavanje ili uklanjanje delegata u programu Outlook za Windows</span><span class="sxs-lookup"><span data-stu-id="946db-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="946db-103">Da biste dodali delegata u programu Outlook za Windows:</span><span class="sxs-lookup"><span data-stu-id="946db-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="946db-104">Kliknite na karticu **datoteka** pored stavke **Postavke naloga**, a zatim odaberite stavku **Delegirani pristup**.</span><span class="sxs-lookup"><span data-stu-id="946db-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="946db-105">Kliknite na dugme " **Dodaj**".</span><span class="sxs-lookup"><span data-stu-id="946db-105">Click on **Add**.</span></span> <span data-ttu-id="946db-106">Ako se **Add** ne pojavi, aktivna veza možda ne postoji između Outlook i Exchange servera.</span><span class="sxs-lookup"><span data-stu-id="946db-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="946db-107">Outlook statusna traka prikazuje status veze.</span><span class="sxs-lookup"><span data-stu-id="946db-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="946db-108">Otkucajte ime osobe koju želite da odredite kao delegata ili pretražite i odaberite ime na listi rezultata pretrage.</span><span class="sxs-lookup"><span data-stu-id="946db-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="946db-109">Delegat mora da bude osoba na Exchange globalnom spisku adresa (GAL) organizacije.</span><span class="sxs-lookup"><span data-stu-id="946db-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="946db-110">Kliknite na dugme " **Dodaj** ," u **redu**.</span><span class="sxs-lookup"><span data-stu-id="946db-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="946db-111">U dijalogu **delegirane dozvole** prihvatite podrazumevane postavke dozvole ili izaberite stavku prilagođeni nivoi pristupa za Exchange fascikle.</span><span class="sxs-lookup"><span data-stu-id="946db-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="946db-112">Ako delegatu treba dozvola za rad samo sa pozivima za sastanke i odgovorima, podrazumevane postavke dozvola kao što je **Delegat prima kopije poruka koje su mi poslate u vezi sa sastankom** .</span><span class="sxs-lookup"><span data-stu-id="946db-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="946db-113">Možete da ostavite postavke dozvole **prijemnog poštanskog sandučeta** na **nijedan**.</span><span class="sxs-lookup"><span data-stu-id="946db-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="946db-114">Pozivi za sastanak i odgovori će otići direktno u prijemno poštansko sanduče delegata.</span><span class="sxs-lookup"><span data-stu-id="946db-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="946db-115">Podrazumevano, delegat se dodeljuje dozvola za **Uređivanje (može da čita, kreira i menja stavke)** u fascikli " **Kalendar** ".</span><span class="sxs-lookup"><span data-stu-id="946db-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="946db-116">Kada delegat odgovori na sastanak u vaše ime, on se automatski dodaje u fasciklu " **Kalendar** ".</span><span class="sxs-lookup"><span data-stu-id="946db-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="946db-117">Da biste poslali poruku da obavestite delegata za promenjene dozvole, potvrdite izbor u polju za potvrdu **automatski Pošalji poruku delegatu za rezimiranje ovih dozvola** .</span><span class="sxs-lookup"><span data-stu-id="946db-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="946db-118">Ako želite, potvrdite izbor u polju za potvrdu **Delegat može da vidi moje privatne stavke** .</span><span class="sxs-lookup"><span data-stu-id="946db-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="946db-119">Ova postavka utiče na sve Exchange fascikle.</span><span class="sxs-lookup"><span data-stu-id="946db-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="946db-120">To obuhvata sve e-poštu, kontakte, kalendare, zadatke, beleške i fascikle naloga.</span><span class="sxs-lookup"><span data-stu-id="946db-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="946db-121">Ne postoji način za odobravanje pristupa privatnim stavkama u samo navedenim fasciklama.</span><span class="sxs-lookup"><span data-stu-id="946db-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="946db-122">Odaberite stavku **u redu**.</span><span class="sxs-lookup"><span data-stu-id="946db-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="946db-123">Poruke poslate sa **dozvolama "Pošalji** u ime" sadrže dozvole delegata i vaša imena pored.</span><span class="sxs-lookup"><span data-stu-id="946db-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="946db-124">Kada se poruka pošalje sa dozvolama "Pošalji kao", pojavljuje se samo vaše ime.</span><span class="sxs-lookup"><span data-stu-id="946db-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="946db-125">Kada dodate nekog kao delegata, može da doda Exchange poštansko sanduče u Outlook profil.</span><span class="sxs-lookup"><span data-stu-id="946db-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="946db-126">Uputstva potražite u članku [upravljanje stavkama pošte i kalendara druge osobe](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span><span class="sxs-lookup"><span data-stu-id="946db-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="946db-127">Da biste uklonili delegata u programu Outlook za Windows:</span><span class="sxs-lookup"><span data-stu-id="946db-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="946db-128">Kliknite na karticu **datoteka** .</span><span class="sxs-lookup"><span data-stu-id="946db-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="946db-129">Izaberite stavku **Postavke naloga** , a zatim **Delegirani pristup**.</span><span class="sxs-lookup"><span data-stu-id="946db-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="946db-130">Odaberite ime delegata za koga želite da promenite dozvole, a zatim kliknite na dugme **Ukloni** , a zatim **u redu**.</span><span class="sxs-lookup"><span data-stu-id="946db-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
