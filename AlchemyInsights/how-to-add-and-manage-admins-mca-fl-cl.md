---
title: Kako se dodaju administratori i upravljaju njima
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755509"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="8d078-102">Kako se dodaju administratori i upravljaju njima</span><span class="sxs-lookup"><span data-stu-id="8d078-102">How to add and manage admins</span></span>

<span data-ttu-id="8d078-103">Na osnovu opisa problema, našli smo rešenje za vas.</span><span class="sxs-lookup"><span data-stu-id="8d078-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="8d078-104">Većina klijenata mogla je samostalno da rešava svoj problem nakon praćenja dokumentacije.</span><span class="sxs-lookup"><span data-stu-id="8d078-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="8d078-105">Da biste upravljali nalogom naplate za Microsoft ugovor o klijentu (MCA), možete da koristite druge uloge sa željenim nivoom pristupa.</span><span class="sxs-lookup"><span data-stu-id="8d078-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="8d078-106">Ove uloge su pored ugrađene uloge usluge Azure koje vam pomažu da kontrolišete resurse.</span><span class="sxs-lookup"><span data-stu-id="8d078-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="8d078-107">**Da biste dodali uloge naplate na portalu Azure:**</span><span class="sxs-lookup"><span data-stu-id="8d078-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="8d078-108">Prijavite se na [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="8d078-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="8d078-109">Potražite *Upravljanje troškovima + naplata*.</span><span class="sxs-lookup"><span data-stu-id="8d078-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="8d078-110">Izaberite stavku Kontrola pristupa (IAM) na opsegu kao što je nalog za naplatu, profil naplate ili odeljak faktura gde želite da date pristup.</span><span class="sxs-lookup"><span data-stu-id="8d078-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="8d078-111">Stranica Kontrola pristupa (IAM) navodi korisnike i grupe dodeljene svakoj ulozi za taj opseg.</span><span class="sxs-lookup"><span data-stu-id="8d078-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="8d078-112">Da biste pristupili korisniku, izaberite stavku **Dodaj** sa vrha stranice.</span><span class="sxs-lookup"><span data-stu-id="8d078-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="8d078-113">Na padajućoj listi *uloga* Izaberite ulogu.</span><span class="sxs-lookup"><span data-stu-id="8d078-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="8d078-114">Unesite e-adresu korisnika kojem želite da date pristup.</span><span class="sxs-lookup"><span data-stu-id="8d078-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="8d078-115">Izaberite stavku **Sačuvaj** da biste dodelili ulogu.</span><span class="sxs-lookup"><span data-stu-id="8d078-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="8d078-116">Da biste uklonili pristup korisniku, izaberite korisnika sa dodelom uloge koju želite da uklonite.</span><span class="sxs-lookup"><span data-stu-id="8d078-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="8d078-117">Izaberite stavku **Ukloni**.</span><span class="sxs-lookup"><span data-stu-id="8d078-117">Select **Remove**.</span></span>

<span data-ttu-id="8d078-118">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="8d078-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="8d078-119">Definicije uloge naplate</span><span class="sxs-lookup"><span data-stu-id="8d078-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="8d078-120">Uloge i zadaci naloga za naplatu</span><span class="sxs-lookup"><span data-stu-id="8d078-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="8d078-121">Prvi koraci uz na za MCA nalog za naplatu</span><span class="sxs-lookup"><span data-stu-id="8d078-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="8d078-122">Proveravaj pristup Microsoft ugovoru o klijentu</span><span class="sxs-lookup"><span data-stu-id="8d078-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
