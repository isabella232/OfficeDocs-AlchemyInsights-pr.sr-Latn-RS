---
title: Dodeljivanje grupa ka usluzi Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885396"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="c73c6-102">Dodeljivanje grupa ka usluzi Azure AD</span><span class="sxs-lookup"><span data-stu-id="c73c6-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="c73c6-103">Da biste dodelili Azure AD grupu sa izvorom autoriteta u Azure AD u ulozi Azure oglasa, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="c73c6-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="c73c6-104">Kreirajte novu grupu – da biste kreirali novu grupu:</span><span class="sxs-lookup"><span data-stu-id="c73c6-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="c73c6-105">Neko.</span><span class="sxs-lookup"><span data-stu-id="c73c6-105">a.</span></span> <span data-ttu-id="c73c6-106">Prijavite se u centar za Azure AD administracije sa **privilegiranom administratorom uloge** ili dozvolama za **Opšte administratore** .</span><span class="sxs-lookup"><span data-stu-id="c73c6-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="c73c6-107">-.</span><span class="sxs-lookup"><span data-stu-id="c73c6-107">b.</span></span> <span data-ttu-id="c73c6-108">Izaberite **Azure Active Directory > grupe > sve grupe > nova grupa**.</span><span class="sxs-lookup"><span data-stu-id="c73c6-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="c73c6-109">trojku.</span><span class="sxs-lookup"><span data-stu-id="c73c6-109">c.</span></span> <span data-ttu-id="c73c6-110">Kreirajte grupu.</span><span class="sxs-lookup"><span data-stu-id="c73c6-110">Create the group.</span></span>

2. <span data-ttu-id="c73c6-111">Dodelite ulogu grupi ili kada se grupa kreira.</span><span class="sxs-lookup"><span data-stu-id="c73c6-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="c73c6-112">Neko.</span><span class="sxs-lookup"><span data-stu-id="c73c6-112">a.</span></span> <span data-ttu-id="c73c6-113">Da biste grupi dodelili ulogu u vreme kreiranja grupe, prebacivanje na opciju preklopnika **Azure oglasa može biti dodeljeno grupi** i Kreiranje grupe.</span><span class="sxs-lookup"><span data-stu-id="c73c6-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="c73c6-114">-.</span><span class="sxs-lookup"><span data-stu-id="c73c6-114">b.</span></span> <span data-ttu-id="c73c6-115">Da biste dodelili ulogu grupi nakon kreiranja, pređite na karticu **dodeljene uloge** za novu grupu i dodelite joj ulogu.</span><span class="sxs-lookup"><span data-stu-id="c73c6-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="c73c6-116">**Upravljanje članstvom grupe koja je dodeljena usluzi Azure AD**</span><span class="sxs-lookup"><span data-stu-id="c73c6-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="c73c6-117">Da biste sprečili podizanje privilegija, podrazumevano, samo privilegovani administratori uloga i globalni administratori mogu da izmene članstvo grupe koja je dodeljena ulozi.</span><span class="sxs-lookup"><span data-stu-id="c73c6-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="c73c6-118">Međutim, oni mogu da izaberu da dodele vlasnika za takvu grupu i delegatu ovaj zadatak.</span><span class="sxs-lookup"><span data-stu-id="c73c6-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="c73c6-119">Više detalja o dodeljivanju grupa oblaka usluzi Azure AD uloge potražite u članku [dodeljivanje uloga u grupi Cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="c73c6-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="c73c6-120">Da biste saznali više o rešavanju problema sa ulogama u oblaku, pogledajte članak [Rešavanje problema sa grupama u oblaku](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="c73c6-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





