---
title: Moderna Azure e-pošta invoicing
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820840"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="d83c8-102">Invoicing e-pošte u Azure</span><span class="sxs-lookup"><span data-stu-id="d83c8-102">Email invoicing in Azure</span></span>

<span data-ttu-id="d83c8-103">Morate da imate ulogu vlasnika ili saradnika na profilu naplate ili njegovom nalogu za naplatu da biste ažurirali željene postavke fakture e-pošte.</span><span class="sxs-lookup"><span data-stu-id="d83c8-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="d83c8-104">Kada omogućite saučesnik, svi korisnici sa ulogama vlasnika, saradnika, čitaoca i menadžera faktura na profilu naplate dobijaju fakturu u e-poruci.</span><span class="sxs-lookup"><span data-stu-id="d83c8-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="d83c8-105">Prijavite se na [Azure portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="d83c8-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="d83c8-106">Potražite **Upravljanje cenom + Naplata**.</span><span class="sxs-lookup"><span data-stu-id="d83c8-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="d83c8-107">Izaberite **stavku Fakture** sa leve strane, a zatim na vrhu stranice izaberite **stavku** Faktura e-poštom.</span><span class="sxs-lookup"><span data-stu-id="d83c8-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="d83c8-108">Ako imate više profila za naplatu, izaberite profil naplate, a zatim izaberite stavku **Dat sajd .**</span><span class="sxs-lookup"><span data-stu-id="d83c8-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="d83c8-109">Izaberite **Ažuriraj**.</span><span class="sxs-lookup"><span data-stu-id="d83c8-109">Select **Update**.</span></span>
6. <span data-ttu-id="d83c8-110">Ako imate više profila za naplatu, izaberite profil naplate, a zatim izaberite stavku **Dat sajd .**</span><span class="sxs-lookup"><span data-stu-id="d83c8-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="d83c8-111">Drugima dajete pristup za prikaz, preuzimanje i plaćanje faktura tako što im dodeljujete ulogu menadžera faktura za MCA ili MPA profil naplate.</span><span class="sxs-lookup"><span data-stu-id="d83c8-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="d83c8-112">Ako ste odlučili da pošaljete fakturu e-poštom, korisnici dobijaju i fakture putem e-pošte.</span><span class="sxs-lookup"><span data-stu-id="d83c8-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="d83c8-113">Prijavite se na [Azure portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="d83c8-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="d83c8-114">Potražite **Upravljanje cenom + Naplata**.</span><span class="sxs-lookup"><span data-stu-id="d83c8-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="d83c8-115">Sa **leve strane izaberite** stavku Profili naplate.</span><span class="sxs-lookup"><span data-stu-id="d83c8-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="d83c8-116">Sa liste profila naplate izaberite profil naplate za koji želite da dodelite ulogu menadžera faktura.</span><span class="sxs-lookup"><span data-stu-id="d83c8-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="d83c8-117">Izaberite **stavku Kontrola pristupa (IAM)** sa leve strane, a zatim **izaberite** stavku Dodaj na vrhu stranice.</span><span class="sxs-lookup"><span data-stu-id="d83c8-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="d83c8-118">Sa padajuće liste Uloga izaberite stavku Upravljač **fakturama**.</span><span class="sxs-lookup"><span data-stu-id="d83c8-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="d83c8-119">Unesite adresu e-pošte korisnika da biste dali pristup.</span><span class="sxs-lookup"><span data-stu-id="d83c8-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="d83c8-120">Kliknite na **dugme Sačuvaj** da biste dodelili ulogu.</span><span class="sxs-lookup"><span data-stu-id="d83c8-120">Select **Save** to assign the role.</span></span>
