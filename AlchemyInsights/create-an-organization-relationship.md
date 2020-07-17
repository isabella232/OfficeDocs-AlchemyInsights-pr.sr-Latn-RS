---
title: Kreiranje relacije između organizacija i Omogućavanje korisnicima da sarađuju sa drugom organizacijom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 2c6cd6a178c6e012bfe1c8d769b037168ffa3254
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862195"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="017b4-102">Kreiranje relacije između organizacija i Omogućavanje korisnicima da sarađuju sa drugom organizacijom</span><span class="sxs-lookup"><span data-stu-id="017b4-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="017b4-103">Sa kontrolne table Microsoft 365 admin Center idite na lokaciju **admin**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="017b4-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="017b4-104">Idite na **organization**  >  **Deljenje**organizacije.</span><span class="sxs-lookup"><span data-stu-id="017b4-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="017b4-105">U okviru **Deljenje organizacija**kliknite na dugme **novo** .</span><span class="sxs-lookup"><span data-stu-id="017b4-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="017b4-106">U **novoj organizaciji odnos**, u okviru za **ime relacije** upišite prepoznatljivo ime za odnos organizacije.</span><span class="sxs-lookup"><span data-stu-id="017b4-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="017b4-107">U okviru " **domeni za deljenje sa** " otkucajte domen za spoljnu Office 365 ili Exchange organizaciju na kojoj želite da vidite svoje kalendare.</span><span class="sxs-lookup"><span data-stu-id="017b4-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="017b4-108">Ako je potrebno da unesete više od jednog domena, razdvojite imena domena zarezom.</span><span class="sxs-lookup"><span data-stu-id="017b4-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="017b4-109">Na primer, contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="017b4-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="017b4-110">Potvrdite izbor u polju za potvrdu **Omogući deljenje informacija o zauzetosti u kalendaru** da biste uključili deljenje kalendara sa domenima koje ste naveli.</span><span class="sxs-lookup"><span data-stu-id="017b4-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="017b4-111">Postavite nivo deljenja za informacije o zauzetosti u kalendaru i podesite koji korisnici mogu da dele informacije o zauzetosti u kalendaru.</span><span class="sxs-lookup"><span data-stu-id="017b4-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="017b4-112">Da biste podesili nivo pristupa zauzetosti, izaberite jednu od sledećih opcija:</span><span class="sxs-lookup"><span data-stu-id="017b4-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="017b4-113">**Kalendarska informacija o zauzetosti sa vremenom**</span><span class="sxs-lookup"><span data-stu-id="017b4-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="017b4-114">**Slobodno/zauzeto kalendar sa vremenom, temom i lokacijom**</span><span class="sxs-lookup"><span data-stu-id="017b4-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="017b4-115">Da biste postavili korisnike koji će deliti informacije o zauzetosti u kalendaru, izaberite jednu od sledećih opcija:</span><span class="sxs-lookup"><span data-stu-id="017b4-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="017b4-116">**Svi u vašoj organizaciji**</span><span class="sxs-lookup"><span data-stu-id="017b4-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="017b4-117">**Navedena bezbednosna grupa**</span><span class="sxs-lookup"><span data-stu-id="017b4-117">**A specified security group**</span></span>  

<span data-ttu-id="017b4-118">Kliknite na dugme " **Pregledaj** " da biste izabrali bezbednosnu grupu sa liste, a zatim kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="017b4-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="017b4-119">Kliknite na dugme **Sačuvaj** da biste kreirali relaciju između organizacija.</span><span class="sxs-lookup"><span data-stu-id="017b4-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="017b4-120">**Napomena:** Konfiguracije izdvojenog tenda ne podržavaju lične kontakte za pronalaženje zauzetosti.</span><span class="sxs-lookup"><span data-stu-id="017b4-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="017b4-121">Kontakti moraju biti uključeni u globalni spisak adresa za pronalaženje zauzetosti na poslu.</span><span class="sxs-lookup"><span data-stu-id="017b4-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="017b4-122">**Za potpuno razumevanje ove teme molimo vas da pročitate:**</span><span class="sxs-lookup"><span data-stu-id="017b4-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="017b4-123">Kreiranje odnosa sa organizacijom u programu Exchange online</span><span class="sxs-lookup"><span data-stu-id="017b4-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="017b4-124">Izmena relacija između organizacija u programu Exchange online</span><span class="sxs-lookup"><span data-stu-id="017b4-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="017b4-125">Uklanjanje organizacionog odnosa u programu Exchange online</span><span class="sxs-lookup"><span data-stu-id="017b4-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
