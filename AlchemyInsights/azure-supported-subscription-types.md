---
title: Podržani tipovi pretplate
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807978"
---
# <a name="supported-subscription-types"></a>Podržani tipovi pretplate

Pregledajte podržane tipove pretplate da biste nastavili dalje.

[Podržani tipovi pretplate](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Prenos vlasništva nad naplatom**

Azure portal kao [administrator naloga](https://ms.portal.azure.com/) za konto naplate koji ima pretplatu koju želite da prenesete

- Pretraga o **upravljanju troškovima + naplata** . Izbor **Pretplata** iz levog okna. U zavisnosti od pristupa, možda ćete morati da izaberete opseg naplate, a zatim **pretplate** ili **Azure pretplate** .
- Izaberite stavku prenos vlasništva naplate za pretplatu koju želite da prenesete
- Unesite e-adresu korisnika koji je administrator naplate naloga koji će biti novi vlasnik za pretplatu, a zatim izaberite stavku **Pošalji zahtev za prenos**
- Korisnik dobija e-poruku sa uputstvima za redigovanje zahteva za prenos. Da biste odobrili zahtev za prenos, korisnik izabere veze u e-poruci i prati uputstva.

Napomena: ako prenesete vlasništvo nad zakupom za pretplatu na nalog korisnika u drugom Azure AD zakupcu, svi zadaci [zasnovane na ulozi (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) dodele za upravljanje resursima u pretplati se trajno uklanjaju. Samo će novi vlasnik imati pristup za upravljanje resursima u pretplati. Više informacija potražite u članku [Prebacivanje pretplate na korisnika u drugom Azure AD zakupcu](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Prenos vlasništva po pretplati**

Preduslovi za prenos vlasništva vlasniљtva na osnovu pretplate (RBAC) da biste upravljali resursima u pretplati, gube pristup. Više informacija o dodavanju postojeće pretplate zakupcu potražite u članku [Povezivanje ili dodavanje Azure aktivnog direktorijuma u Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Prenos pretplate sa postojećim Neplaćeni iznos iz trenutnog ciklusa naplate neće se prenositi na novi instrument plaćanja na novom nalogu. Jedine informacije dostupne korisnicima na novom nalogu su troškovi za vašu pretplatu. Ostatak istorije upotrebe i naplate se ne prenosi pomoću pretplate.
- Pretplata na prenos vlasništva nad imovinom na Enterprise sporazumu je trenutno podržana samo na portalu Enterprise sporazuma
- Prenošenje pretplate orijentisane na kredit kao što je Visual Studio, BizSpark, Microsoft partner mreža za novog korisnika zahtevaju da imate Visual Studio/Microsoft partner mrežnu licencu da biste prihvatili zahtev za prenos
- Svi resursi kao što su virtuelne mašine, diskovi i Veb lokacije, uspešno se prebacuju na novi nalog. Sledeći resursi mogu da se utiču na prenos pretplate preko zakupca:

**Usluge Azure AD Domain**

Sefovi ključa za Azure

- Moguće je uticati na [SQL srodni korisnici i baze podataka](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) , naročito ako korisnik koristi Azure Active Directory za potvrdu identiteta
- **Usluge aplikacije** podešene pomoću usluge Azure Active Directory potvrda identiteta može biti uticalo
- **Vizuelni studio Team** Usluge usluge koje su povezane sa uslugom Azure mogu privremeno da izgube pristup kada se poveže povezana Azure pretplata

**Preporučeni dokumenti**

Koraci posle prihvatanja vlasništva naplata:

- Da biste zadržali vlasništvo nad naplatom, ali promenili tip pretplate, pogledajte: [Prebacivanje Azure pretplate na drugu ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenošenje vizuelnog studija, Microsoft partner Network (MPN) i isplata dok idete na delanje Dev/test](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prenos vlasništva nad imovinom za Enterprise ugovor (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Najčešća pitanja o vlasništvu prenosa](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Rešavanje problema sa vlasništvom prenosa](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)