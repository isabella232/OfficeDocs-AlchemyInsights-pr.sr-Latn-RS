---
title: Prenos vlasništva nad naplatom za uslugu Azure
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
- "9003560"
- "6849"
ms.openlocfilehash: 803d0105ad2bbaf2b18cea6aa556b6af5e09cb2d41812d4747aa703e6e7d7780
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036110"
---
# <a name="transfer-azure-billing-ownership"></a>Prenos vlasništva nad naplatom za uslugu Azure

Prijavite se na [Azure portal](https://portal.azure.com/) kao administrator naloga za naplatu koji ima pretplatu koju želite da prenesete. Ako niste sigurni u to da li ste administrator ili ako treba da utvrdite ko jeste, pogledajte članak [Odredite administratora naloga za naplatu](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Potražite _Upravljanje cenom + Naplata_.
1. Izaberite **Pretplate** iz levog okna. U zavisnosti od pristupa, možda ćete morati da izaberete opseg naplate, a zatim **Pretplate** ili **Azure pretplate**.
1. Izaberite **Prenos vlasništva nad naplatom** za pretplatu koju želite da prenesete.
1. Unesite adresu e-pošte korisnika koji je administrator naplate za nalog koji će biti novi vlasnik pretplate, a zatim izaberite **pošalji zahtev za prenos**.
1. Korisnik dobija e-poruku sa uputstvima da pregleda vaš zahtev za prenos. Da bi odobrio zahtev za prenos, korisnik odabira vezu u e-poruci i prati uputstva.

Imajte u vidu da se sva zaduženja sa [kontrolom pristupa na osnovu uloga (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) za upravljanje resursima u pretplati trajno uklanjanju ako prenesete vlasništvo nad naplatom vaše pretplate na korisnički nalog u drugom Azure AD zakupcu. Samo će novi vlasnik imati pristup za upravljanje resursima u pretplati. Za više informacija o tome kako da promenite direktorijum za pretplatu, pogledajte [Prenos pretplate na korisnika u drugom Azure AD zakupcu ](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Važan uticaj na vaše fakture**_: Ako ste preneli vlasništvo nad naplatom za Azure pretplatu, troškovi će biti srazmerni. Moći ćete da pristupite fakturama na sledeći način:  

1. Izaberite vašu pretplatu sa  [Stranice za pretplate](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)  u Azure portalu kao  [ korisnik sa pristupom fakturama](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), a zatim izaberite  **Fakture**.
1. Kliknite na  **Preuzmi fakturu**  da biste videli kopiju fakture u PDF formatu. Ako kaže  _Nije dostupno_, pogledajte  [Zašto se ne prikazuje faktura za poslednji period naplate?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).
1. Možete da vidite i dnevno korišćenje tako što ćete kliknuti na **period naplate** da biste dobili PDF vaše fakture i kopiju datoteke o detaljnom dnevnom korišćenju (.CSV) Za više informacija, pogledajte  [Preuzmite fakturu i podatke o korišćenju](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Preporučeni dokumenti**

- [Prenesite vlasništvo nad naplatom za Azure pretplatu na drugi nalog](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [O prenosu vlasništva nad naplatom za Azure pretplatu](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Prenos pretplata za projektante/testiranje za Visual Studio, Microsoft Partner Network (MPN) i Plaćanje po utrošku](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prenos vlasništva – najčešća pitanja](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Rešavanje problema u vezi sa prenosom vlasništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
