---
title: Konfigurisanje usluge odredbe
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484042"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="8f9aa-102">Konfigurisanje usluge odredbe</span><span class="sxs-lookup"><span data-stu-id="8f9aa-102">Configuring the Provision service</span></span>

<span data-ttu-id="8f9aa-103">Za automatizovano obezbeđivanje rada na poslu, Azure AD zahteva važeće akreditive koje mu omogućuju da se poveže sa API-jem veb uslugama posla.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="8f9aa-104">Dodatno, dugme Testiraj vezu na radnom mestu za dodelu oglasa korisnika takođe proverava valjanost ako je u mogućnosti da se poveže sa agentom Azure AD Connect za obezbeđivanje povezivanja sa agentom za AD.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="8f9aa-105">Ako Azure portal vraća grešku prilikom čuvanja akreditiva, slijedite sledeće navedene korake:</span><span class="sxs-lookup"><span data-stu-id="8f9aa-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="8f9aa-106">Potvrdite da ste podesili korisnički nalog sistema za integraciju u operativnom sistemu za integraciju kao što je navedeno u odeljku uputstvo [Konfiguriši korisnika sistema za integraciju u radnom toku](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="8f9aa-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="8f9aa-107">Potvrdite da je usluga Azure veze za obezbeđivanje OGLAŠAVANJA uključena i da je pokrenuta na lokalnom Windows serveru pomoću konzole Management Console.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="8f9aa-108">Status agenta možete da potvrdite i tako što ćete kliknuti na dugme prikaz lokalnog agensa.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="8f9aa-109">Uverite se da unosite vrednost za polje "korisničko ime radnog dana" pomoću formata username@workday-zakupca.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="8f9aa-110">Ako nedostaje radni dan-zakupac, potvrda radnog dana ne uspeva.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="8f9aa-111">Ako podešavate integraciju sa zakupcem radnog dana, zabeležite planirana vremena za smanjenje radnog dana.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="8f9aa-112">Radni dan je već zakazao vreme za svoje stanare za implementaciju tokom vikenda (obično od petka uveče do subote ujutru) i problema sa povezivanjem tokom ovog prozora za smanjivanje je poznat problem koji se automatski rešava čim se svi stanari primene vrate na mreži.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="8f9aa-113">U retkim slučajevima možete da vidite i ovu grešku ako je lozinka sistema za integraciju korisnik promenjen zbog osvežavanja zakupca ili ako je nalog u zaključanom ili isteklom stanju.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="8f9aa-114">Proverite status korisnika sistema za integraciju sa vašim radnim danom administratorom.</span><span class="sxs-lookup"><span data-stu-id="8f9aa-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="8f9aa-115">Za više detalja o konfigurisanju radnog vremena za automatizovano obezbeđivanje pogledajte [članak uputstvo: konfigurisanje radnog dana za automatsko obezbeđivanje korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="8f9aa-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
