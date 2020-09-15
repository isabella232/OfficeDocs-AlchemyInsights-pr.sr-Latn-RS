---
title: Identifikovanje IP adrese i klijenta u evidenciji nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668324"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="8951d-102">Identifikovanje IP adrese i klijenta u evidenciji nadzora</span><span class="sxs-lookup"><span data-stu-id="8951d-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="8951d-103">IP adresa koja odgovara aktivnosti Microsoft 365 korisnika ili administratora je prikazana u evidenciji nadzora.</span><span class="sxs-lookup"><span data-stu-id="8951d-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="8951d-104">Informacije o klijentu se takođe evidentiraju.</span><span class="sxs-lookup"><span data-stu-id="8951d-104">The client information is also logged.</span></span> <span data-ttu-id="8951d-105">Evo koraka za identifikovanje takvih informacija</span><span class="sxs-lookup"><span data-stu-id="8951d-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="8951d-106">Prijavite se u [Microsoft 365 Security & centar za usaglašenost](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="8951d-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="8951d-107">Idite na stranicu **Search**  >  **Pretraga evidencije nadgledanja** za pretraživanje.</span><span class="sxs-lookup"><span data-stu-id="8951d-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="8951d-108">Ako ste zainteresovani za određenu aktivnost, izaberite je sa liste **aktivnosti** .</span><span class="sxs-lookup"><span data-stu-id="8951d-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="8951d-109">Ako to ne uradite, sve aktivnosti će biti vraćene za izabranog korisnika (podrazumevana postavka).</span><span class="sxs-lookup"><span data-stu-id="8951d-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="8951d-110">**Napomena**: neke aktivnosti možda neće biti dostupne u meniju " **aktivnosti** "; Međutim, te stavke nadgledanja će biti vraćene ako je izabrana opcija **Prikaži rezultate za sve aktivnosti** (podrazumevana postavka).</span><span class="sxs-lookup"><span data-stu-id="8951d-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="8951d-111">Navedite korisničko ime u polju **Korisnici** , izaberite odgovarajući opseg datuma za aktivnost, a zatim kliknite na dugme **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="8951d-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="8951d-112">U rezultatima možete da vidite IP adresu za tu aktivnost u oknu sa rezultatima.</span><span class="sxs-lookup"><span data-stu-id="8951d-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="8951d-113">Izaberite zapis nadzora da biste videli detaljne informacije u razgledanju **detalja** (na primer klijenta, korisnika koji je izvršio radnju itd.).</span><span class="sxs-lookup"><span data-stu-id="8951d-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="8951d-114">Više informacija potražite u članku [PRONALAŽENJE IP adrese računara korišćenog za pristup kompromitovanim nalozima](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="8951d-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
