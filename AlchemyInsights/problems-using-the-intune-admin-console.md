---
title: Problemi pri korišćenju funkcije Intune admin Console
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555876"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="b5298-102">Problemi pri korišćenju funkcije Intune admin Console</span><span class="sxs-lookup"><span data-stu-id="b5298-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="b5298-103">**"Pristup je odbijen" prilikom kretanja administratorskog portala Intune.**</span><span class="sxs-lookup"><span data-stu-id="b5298-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="b5298-104">Ako ste član "Intune" prilagođene uloge, uverite se da je na nalog dodeljen licencu za Intune ili poslovnu mobilnost (EMS).</span><span class="sxs-lookup"><span data-stu-id="b5298-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="b5298-105">Ako koristite upravljač za konfiguraciju za upravljanje uređajima, proverite da niste deo funkcije "Intune korisnika" za upravljač konfiguracije MDM.</span><span class="sxs-lookup"><span data-stu-id="b5298-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="b5298-106">Proverite da li vam je dodeljena odgovarajuća dozvola za kontrolu administracije zasnovana na ulogama (RBAC) u oštricom za Intune.</span><span class="sxs-lookup"><span data-stu-id="b5298-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="b5298-107">Provera grupe koja se koristi nije lista distribucije.</span><span class="sxs-lookup"><span data-stu-id="b5298-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="b5298-108">Intune na Azure portalu podržava samo korisničke naloge koji pripadaju samo Azure bezbednosnim grupama aktivnog direktorijuma.</span><span class="sxs-lookup"><span data-stu-id="b5298-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="b5298-109">Pregledajte grupe u > **Intune**  >  ili u**grupi**Azure portala > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="b5298-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="b5298-110">**Korisnik ima previše dozvola za dodeljenu ulogu Intune**</span><span class="sxs-lookup"><span data-stu-id="b5298-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="b5298-111">Posavetuje korisnika da ide u " **Intune**  >  **Intune" uloge**  >  **moje dozvole**  >  **Izvezi** da pregleda dodeljene dozvole.</span><span class="sxs-lookup"><span data-stu-id="b5298-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="b5298-112">**U ulogu je dodata grupa opsega, ali korisnici u toj ulozi i dalje vide druge korisnike ili uređaje.**</span><span class="sxs-lookup"><span data-stu-id="b5298-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="b5298-113">Grupe opsega ne filtriraju korisnike ili uređaje.</span><span class="sxs-lookup"><span data-stu-id="b5298-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="b5298-114">Grupe opsega:</span><span class="sxs-lookup"><span data-stu-id="b5298-114">Scope groups:</span></span>

- <span data-ttu-id="b5298-115">Ograničite pristup kome korisnici mogu da dodeljuju smernice ili aplikacije.</span><span class="sxs-lookup"><span data-stu-id="b5298-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="b5298-116">Dozvoli samo određenim korisnicima da pokrenu udaljene zadatke na uređajima.</span><span class="sxs-lookup"><span data-stu-id="b5298-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="b5298-117">Više informacija o grupama opsega potražite u članku [Kontrola pristupa zasnovana na ulozi (RBAC) sa programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="b5298-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="b5298-118">**Dodao sam korisnika u ulogu Intune, ali i dalje imaju potpuni pristup usluzi Intune admin Console.**</span><span class="sxs-lookup"><span data-stu-id="b5298-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="b5298-119">Dođite do Intune > **korisnika** na Azure portalu i proverite da li korisnik nije dodeljen ni jednom od sledećih uloga na Azure portalu:</span><span class="sxs-lookup"><span data-stu-id="b5298-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="b5298-120">Globalni administratorski</span><span class="sxs-lookup"><span data-stu-id="b5298-120">Global administrator</span></span>
- <span data-ttu-id="b5298-121">Administrator Intune usluge</span><span class="sxs-lookup"><span data-stu-id="b5298-121">Intune service administrator</span></span>
- <span data-ttu-id="b5298-122">SharePoint administratoru</span><span class="sxs-lookup"><span data-stu-id="b5298-122">SharePoint administrator</span></span>

<span data-ttu-id="b5298-123">Više informacija potražite u članku [Kontrola pristupa zasnovana na ulogama (RBAC) sa programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="b5298-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="b5298-124">**Problemi sa pristupom**</span><span class="sxs-lookup"><span data-stu-id="b5298-124">**Access Issues**</span></span>

<span data-ttu-id="b5298-125">Više informacija potražite u članku [ne možete da se prijavite na Office 365, Azure ili Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="b5298-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>