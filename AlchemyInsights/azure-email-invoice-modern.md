---
title: Moderno Azure fakturisanje e-pošte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922142"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="de681-102">Slanje e-pošte u Azure</span><span class="sxs-lookup"><span data-stu-id="de681-102">Email invoicing in Azure</span></span>

<span data-ttu-id="de681-103">Da biste ažurirali željene postavke fakture e-pošte, morate imati ulogu vlasnika ili uloge saradnika.</span><span class="sxs-lookup"><span data-stu-id="de681-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="de681-104">Kada se odlučite, svi korisnici sa ulogama, saradnikom, čitačima i ulozi Menadžera za fakture na profilu naplate dobiće svoju fakturu e-poštom.</span><span class="sxs-lookup"><span data-stu-id="de681-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="de681-105">Prijavite se na [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="de681-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="de681-106">Potražite **Upravljanje troškovima + naplata**.</span><span class="sxs-lookup"><span data-stu-id="de681-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="de681-107">Izaberite stavku **fakture** sa leve strane, a zatim na vrhu stranice izaberite stavku **faktura e-pošta** .</span><span class="sxs-lookup"><span data-stu-id="de681-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="de681-108">Ako imate više profila naplate, izaberite profil naplate, a zatim izaberite stavku **saglasnost**.</span><span class="sxs-lookup"><span data-stu-id="de681-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="de681-109">Izaberite stavku **Ažuriraj**.</span><span class="sxs-lookup"><span data-stu-id="de681-109">Select **Update**.</span></span>
6. <span data-ttu-id="de681-110">Ako imate više profila naplate, izaberite profil naplate, a zatim izaberite stavku **saglasnost**.</span><span class="sxs-lookup"><span data-stu-id="de681-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="de681-111">Drugima dajete pristup da prikažu, preuzmu i plaćaju fakture tako što im dodeljuju ulogu Menadžera za fakture za profil naplate za MCA ili MPA.</span><span class="sxs-lookup"><span data-stu-id="de681-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="de681-112">Ako ste odlučili da nabavite fakturu u e-poruci, korisnici takođe šalju fakture e-poštom.</span><span class="sxs-lookup"><span data-stu-id="de681-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="de681-113">Prijavite se na [Azure portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="de681-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="de681-114">Potražite **Upravljanje troškovima + naplata**.</span><span class="sxs-lookup"><span data-stu-id="de681-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="de681-115">Izaberite **profile naplate** sa leve strane.</span><span class="sxs-lookup"><span data-stu-id="de681-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="de681-116">Na listi profili naplate izaberite profil naplate za koji želite da dodelite ulogu Menadžera za fakture.</span><span class="sxs-lookup"><span data-stu-id="de681-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="de681-117">Izaberite stavku **Kontrola pristupa** sa leve strane, a zatim izaberite stavku **Dodaj** sa vrha stranice.</span><span class="sxs-lookup"><span data-stu-id="de681-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="de681-118">Na padajućoj listi uloga izaberite stavku **Upravljač fakturama**.</span><span class="sxs-lookup"><span data-stu-id="de681-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="de681-119">Unesite e-adresu korisnika za pružanje pristupa.</span><span class="sxs-lookup"><span data-stu-id="de681-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="de681-120">Izaberite stavku **Sačuvaj** da biste dodelili ulogu.</span><span class="sxs-lookup"><span data-stu-id="de681-120">Select **Save** to assign the role.</span></span>
