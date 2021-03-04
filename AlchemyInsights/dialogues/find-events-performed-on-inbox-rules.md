---
title: Pronalaženje događaja koji se izvršavaju na pravilima prijemnog poštanskog sandučeta
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430015"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="e5a5c-102">Pronalaženje događaja koji se izvršavaju na pravilima prijemnog poštanskog sandučeta</span><span class="sxs-lookup"><span data-stu-id="e5a5c-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="e5a5c-103">Kada se pravila prijemnog poštanskog sandučeta kreiraju, menjaju ili brišu, događaji se snimaju u evidenciji nadzora.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="e5a5c-104">Evo kako da ih pregledate:</span><span class="sxs-lookup"><span data-stu-id="e5a5c-104">Here's how to review them:</span></span>

1. <span data-ttu-id="e5a5c-105">Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="e5a5c-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="e5a5c-106">Izaberite stavku Pretraga > pretraga nadzora.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e5a5c-107">Ako vidite obaveštenje koje treba da uključite u nadzor, odmah ga uključite.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="e5a5c-108">Ako ova funkcija nije uključena, rezultati pretrage neće moći da izvuku podatke iz prethodnih datuma.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="e5a5c-109">Izaberite polje aktivnosti i pronađite usluge Exchange poštanskog sandučeta, a zatim izaberite New-InboxRule Kreirajte pravilo za Prijemno sanduče iz programa Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="e5a5c-110">Kada završite, kliknite izvan okna da biste smanjili okno "aktivnosti".</span><span class="sxs-lookup"><span data-stu-id="e5a5c-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="e5a5c-111">Navedite opseg datuma, a zatim u polju korisnici izaberite korisničko ime za korisnika kojeg želite da istražite.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="e5a5c-112">Možete da izaberete više korisnika odjednom.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="e5a5c-113">Izaberite stavku Pretraži.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-113">Select Search.</span></span> <span data-ttu-id="e5a5c-114">Aktivnosti se pojavljuju u okviru rezultati.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="e5a5c-115">Da biste prikazali detalje, izaberite aktivnost, a zatim izaberite stavku još informacija.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="e5a5c-116">U odeljku parametri možete da vidite ime pravila, postavljene uslove i radnje koje će pravilo preduzeti.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="e5a5c-117">Da biste saznali više, pogledajte članak pretraga Office 365 evidencije nadzora radi rešavanja problema sa uobičajenim scenarijima.</span><span class="sxs-lookup"><span data-stu-id="e5a5c-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>