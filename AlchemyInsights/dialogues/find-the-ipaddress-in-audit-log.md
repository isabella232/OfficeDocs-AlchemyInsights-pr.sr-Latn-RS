---
title: Pronađite IP adresu u evidenciji nadzora
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429789"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="2db3a-102">Pronađite IP adresu u evidenciji nadzora</span><span class="sxs-lookup"><span data-stu-id="2db3a-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="2db3a-103">IP adresa koja odgovara aktivnoj aktivnosti korisnika ili administratora prikazuje se u evidenciji nadzora.</span><span class="sxs-lookup"><span data-stu-id="2db3a-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="2db3a-104">Informacije o klijentu se takođe evidentiraju.</span><span class="sxs-lookup"><span data-stu-id="2db3a-104">The client information is also logged.</span></span> <span data-ttu-id="2db3a-105">Evo kako da identifikujete IP adresu:</span><span class="sxs-lookup"><span data-stu-id="2db3a-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="2db3a-106">Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="2db3a-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="2db3a-107">Izaberite **stavku**  >  **[Pretraga evidencije nadzora](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="2db3a-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="2db3a-108">Ako vidite obaveštenje koje treba da uključite u nadzor, odmah ga uključite.</span><span class="sxs-lookup"><span data-stu-id="2db3a-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="2db3a-109">Ako ova funkcija nije omogućena, rezultati pretrage neće moći da izvuku podatke iz prethodnih datuma.</span><span class="sxs-lookup"><span data-stu-id="2db3a-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="2db3a-110">Ako ste zainteresovani za određenu aktivnost, izaberite je sa liste **aktivnosti** . u suprotnom, podrazumevano će sve aktivnosti biti vraćene za izabranog korisnika.</span><span class="sxs-lookup"><span data-stu-id="2db3a-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="2db3a-111">Imajte u vidu da određene aktivnosti možda nisu dostupne za izbor iz menija " **aktivnosti** "; Međutim, te stavke nadgledanja će biti vraćene ako je izabrana opcija **Prikaži rezultate za sve aktivnosti** (podrazumevana postavka).</span><span class="sxs-lookup"><span data-stu-id="2db3a-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="2db3a-112">Navedite opseg datuma i u polju **Korisnici** izaberite korisničko ime za korisnika kojeg želite da istražite.</span><span class="sxs-lookup"><span data-stu-id="2db3a-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="2db3a-113">Izaberite stavku **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="2db3a-113">Select **Search**.</span></span> <span data-ttu-id="2db3a-114">Aktivnosti se pojavljuju u okviru **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="2db3a-114">The activities appear under **Results**.</span></span> <span data-ttu-id="2db3a-115">Možete da vidite IP adresu za svaku aktivnost.</span><span class="sxs-lookup"><span data-stu-id="2db3a-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="2db3a-116">Da biste prikazali detalje, izaberite aktivnost, a zatim izaberite stavku **još informacija**.</span><span class="sxs-lookup"><span data-stu-id="2db3a-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="2db3a-117">Da biste saznali više, pogledajte članak pretraga [Office 365 evidencije nadzora radi rešavanja problema sa uobičajenim scenarijima](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="2db3a-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>