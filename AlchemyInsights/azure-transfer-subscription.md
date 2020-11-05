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
# <a name="transfer-azure-billing-ownership"></a>Prenos Azure vlasništva

Prijavite se na [Azure portal](https://portal.azure.com/) kao administrator naloga naplate koji ima pretplatu koju želite da prenesete. Ako niste sigurni da li ste i administrator ili ako treba da utvrdite ko je, pogledajte odeljak [Utvrđivanje administratora za naplatu naloga](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Pretraga o **upravljanju troškovima + naplata**.
- Izaberite stavku **pretplate** iz levog okna. U zavisnosti od pristupa, možda ćete morati da izaberete opseg naplate, a zatim **pretplate** ili **Azure pretplate**.
- Izaberite stavku **prenos vlasništva naplate** za pretplatu koju želite da prenesete
- Unesite e-adresu korisnika koji je administrator naplate naloga koji će biti novi vlasnik za pretplatu, a zatim izaberite stavku **Pošalji zahtev za prenos**
- Korisnik dobija e-poruku sa uputstvima za redigovanje zahteva za prenos. Da biste odobrili zahtev za prenos, korisnik izabere veze u e-poruci i prati uputstva.

**Napomena** : ako prenesete vlasništvo nad zakupom za pretplatu na nalog korisnika u drugom AZURE AD zakupcu, svi zadaci [zasnovane na ulozi (rbac)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)dodele za upravljanje resursima u pretplati se trajno uklanjaju. Samo će novi vlasnik imati pristup za upravljanje resursima u pretplati. Više informacija potražite u članku [Prebacivanje pretplate na korisnika u drugom Azure AD zakupcu](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Preporučeni dokumenti**

- [Prebacivanje vlasništva nad naplatom na Azure pretplatu na drugi nalog](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [O prenosu vlasništva nad naplatom za Azure pretplatu](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Prenošenje vizuelnog studija, Microsoft partner Network (MPN) i isplata dok idete na delanje Dev/test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Najčešća pitanja o vlasništvu prenosa](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Rešavanje problema sa vlasništvom prenosa](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
