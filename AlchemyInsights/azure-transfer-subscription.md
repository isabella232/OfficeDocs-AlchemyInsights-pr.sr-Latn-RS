---
title: Prenos Azure vlasništva
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922168"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="3757e-102">Prenos Azure vlasništva</span><span class="sxs-lookup"><span data-stu-id="3757e-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="3757e-103">Prijavite se na [Azure portal](https://portal.azure.com/) kao administrator naloga naplate koji ima pretplatu koju želite da prenesete.</span><span class="sxs-lookup"><span data-stu-id="3757e-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="3757e-104">Ako niste sigurni da li ste i administrator ili ako treba da utvrdite ko je, pogledajte odeljak [Utvrđivanje administratora za naplatu naloga](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="3757e-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="3757e-105">Pretraga o **upravljanju troškovima + naplata**.</span><span class="sxs-lookup"><span data-stu-id="3757e-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="3757e-106">Izaberite stavku **pretplate** iz levog okna.</span><span class="sxs-lookup"><span data-stu-id="3757e-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="3757e-107">U zavisnosti od pristupa, možda ćete morati da izaberete opseg naplate, a zatim **pretplate** ili **Azure pretplate**.</span><span class="sxs-lookup"><span data-stu-id="3757e-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="3757e-108">Izaberite stavku **prenos vlasništva naplate** za pretplatu koju želite da prenesete</span><span class="sxs-lookup"><span data-stu-id="3757e-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="3757e-109">Unesite e-adresu korisnika koji je administrator naplate naloga koji će biti novi vlasnik za pretplatu, a zatim izaberite stavku **Pošalji zahtev za prenos**</span><span class="sxs-lookup"><span data-stu-id="3757e-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="3757e-110">Korisnik dobija e-poruku sa uputstvima za redigovanje zahteva za prenos.</span><span class="sxs-lookup"><span data-stu-id="3757e-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="3757e-111">Da biste odobrili zahtev za prenos, korisnik izabere veze u e-poruci i prati uputstva.</span><span class="sxs-lookup"><span data-stu-id="3757e-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="3757e-112">**Napomena** : ako prenesete vlasništvo nad zakupom za pretplatu na nalog korisnika u drugom AZURE AD zakupcu, svi zadaci [zasnovane na ulozi (rbac)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)dodele za upravljanje resursima u pretplati se trajno uklanjaju.</span><span class="sxs-lookup"><span data-stu-id="3757e-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="3757e-113">Samo će novi vlasnik imati pristup za upravljanje resursima u pretplati.</span><span class="sxs-lookup"><span data-stu-id="3757e-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="3757e-114">Više informacija potražite u članku [Prebacivanje pretplate na korisnika u drugom Azure AD zakupcu](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="3757e-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="3757e-115">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="3757e-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="3757e-116">Prebacivanje vlasništva nad naplatom na Azure pretplatu na drugi nalog</span><span class="sxs-lookup"><span data-stu-id="3757e-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="3757e-117">O prenosu vlasništva nad naplatom za Azure pretplatu</span><span class="sxs-lookup"><span data-stu-id="3757e-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="3757e-118">Prenošenje vizuelnog studija, Microsoft partner Network (MPN) i isplata dok idete na delanje Dev/test</span><span class="sxs-lookup"><span data-stu-id="3757e-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="3757e-119">Najčešća pitanja o vlasništvu prenosa</span><span class="sxs-lookup"><span data-stu-id="3757e-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="3757e-120">Rešavanje problema sa vlasništvom prenosa</span><span class="sxs-lookup"><span data-stu-id="3757e-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
