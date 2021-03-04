---
title: Čitanje evidencija nadzora za izbrisane događaje
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429824"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="89d77-102">Čitanje evidencija nadzora za izbrisane događaje</span><span class="sxs-lookup"><span data-stu-id="89d77-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="89d77-103">Evo kako ovo da uradite:</span><span class="sxs-lookup"><span data-stu-id="89d77-103">Here's how to do this:</span></span>

1. <span data-ttu-id="89d77-104">Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="89d77-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="89d77-105">Izaberite **stavku**  >  [**Pretraga evidencije nadzora**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="89d77-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="89d77-106">Ako vidite obaveštenje koje treba da uključite, odmah ga uključite.</span><span class="sxs-lookup"><span data-stu-id="89d77-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="89d77-107">Ako funkcija nije uključena, rezultati pretrage neće moći da izvuku podatke iz prethodnih datuma.</span><span class="sxs-lookup"><span data-stu-id="89d77-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="89d77-108">Izaberite stavku **aktivnosti**, a zatim pronađite **aktivnosti Exchange poštanskog sandučeta**.</span><span class="sxs-lookup"><span data-stu-id="89d77-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="89d77-109">Izaberite stavku **izbrisane poruke iz izbrisane** fascikle i premestili ste opcije fascikle " **Izbrisane stavke** ".</span><span class="sxs-lookup"><span data-stu-id="89d77-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="89d77-110">Kada završite, kliknite izvan okna da biste smanjili okno " **aktivnosti** ".</span><span class="sxs-lookup"><span data-stu-id="89d77-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="89d77-111">Navedite opseg datuma, a zatim u okviru **Korisnici** izaberite korisničko ime za korisnika kojeg želite da istražite.</span><span class="sxs-lookup"><span data-stu-id="89d77-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="89d77-112">Možete da izaberete više korisnika odjednom.</span><span class="sxs-lookup"><span data-stu-id="89d77-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="89d77-113">Izaberite stavku **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="89d77-113">Select **Search**.</span></span> <span data-ttu-id="89d77-114">Aktivnosti se pojavljuju u okviru **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="89d77-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="89d77-115">Da biste prikazali detalje, izaberite aktivnost, a zatim izaberite stavku **još informacija**.</span><span class="sxs-lookup"><span data-stu-id="89d77-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="89d77-116">Dodatne informacije o izbrisanim stavkama, kao što je red za temu i lokacija stavke kada je izbrisana, prikazuje se u polju " **Afekcteditem** ".</span><span class="sxs-lookup"><span data-stu-id="89d77-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="89d77-117">Ne možete da vratite izbrisane stavke pomoću funkcije evidencije nadzora.</span><span class="sxs-lookup"><span data-stu-id="89d77-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="89d77-118">Da biste vratili izbrisane stavke, pogledajte članak [oporavak izbrisanih stavki ili e-pošte u programu Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="89d77-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="89d77-119">Da biste saznali više, pogledajte članak [Pretraga Office 365 evidencije nadzora radi rešavanja problema sa uobičajenim scenarijima](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="89d77-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
