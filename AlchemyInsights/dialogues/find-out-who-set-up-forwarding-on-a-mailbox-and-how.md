---
title: Saznajte ko je podesio prosleđivanje u poštanskom sandučetu i na koji način
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429993"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="1a34a-102">Saznajte ko je podesio prosleđivanje u poštanskom sandučetu i na koji način</span><span class="sxs-lookup"><span data-stu-id="1a34a-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="1a34a-103">Ako je spoljni prosleđivanje postavljen na poštansko sanduče, aktivnost se nadgleda kao deo Set-Mailbox cmdlet zapisa.</span><span class="sxs-lookup"><span data-stu-id="1a34a-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="1a34a-104">Evo kako da pronađete aktivnost u evidenciji nadzora:</span><span class="sxs-lookup"><span data-stu-id="1a34a-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="1a34a-105">Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="1a34a-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="1a34a-106">Izaberite **stavku** >  **Pretraga evidencije nadzora**.</span><span class="sxs-lookup"><span data-stu-id="1a34a-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="1a34a-107">Ako vidite obaveštenje koje treba da uključite u nadzor, odmah ga uključite.</span><span class="sxs-lookup"><span data-stu-id="1a34a-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="1a34a-108">Ako ova funkcija nije uključena, rezultati pretrage neće moći da izvuku podatke iz prethodnih datuma.</span><span class="sxs-lookup"><span data-stu-id="1a34a-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="1a34a-109">Proverite da li je polje **aktivnosti** podešeno da **prikazuje rezultate za sve aktivnosti** (podrazumevano).</span><span class="sxs-lookup"><span data-stu-id="1a34a-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="1a34a-110">Navedite opseg datuma.</span><span class="sxs-lookup"><span data-stu-id="1a34a-110">Specify the date range.</span></span> <span data-ttu-id="1a34a-111">Nije potrebno da navedete korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="1a34a-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="1a34a-112">Izaberite stavku **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="1a34a-112">Select **Search**.</span></span> <span data-ttu-id="1a34a-113">Aktivnosti se pojavljuju u okviru **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="1a34a-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="1a34a-114">Izaberite stavke **Filtriraj rezultate**, a zatim u polju Filter **aktivnosti** unesite **podešeno poštansko sanduče** .</span><span class="sxs-lookup"><span data-stu-id="1a34a-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="1a34a-115">Ovo daje sve aktivnosti **za skupa poštanskog sandučeta** .</span><span class="sxs-lookup"><span data-stu-id="1a34a-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="1a34a-116">Da biste prikazali detalje, izaberite aktivnost, a zatim izaberite stavku **još informacija**.</span><span class="sxs-lookup"><span data-stu-id="1a34a-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="1a34a-117">U okviru **Parametri** možete da vidite Prosleđivanje e-adrese koja je postavljena na poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="1a34a-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="1a34a-118">**ID** korisnika predstavlja korisnika koji je podesio spoljnu prosleđivanje na poštansko sanduče.</span><span class="sxs-lookup"><span data-stu-id="1a34a-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="1a34a-119">Da biste saznali više, pogledajte članak [Pretraga Office 365 evidencije nadzora radi rešavanja problema sa uobičajenim scenarijima](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="1a34a-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>