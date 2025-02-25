---
title: Podržani tipovi pretplata
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
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072174"
---
# <a name="supported-subscription-types"></a>Podržani tipovi pretplata

Pregledajte podržane tipove pretplata da biste nastavili dalje.

[Podržani tipovi pretplata](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Prenos vlasništva nad naplatom**

Azure portal kao [administ za](https://ms.portal.azure.com/) nalog za naplatu koji ima pretplatu koju želite da prenesete

- Pretražujte na stranici **Upravljanje cenom + Naplata**. Izaberite **stavku Pretplate iz** levog okna. U zavisnosti od pristupa, možda ćete morati da izaberete opseg naplate, a zatim **Pretplate** ili **Azure pretplate**.
- Izaberite stavku "Prenos vlasništva nad naplatom" za pretplatu koju želite da prenesete
- Unesite adresu e-pošte korisnika koji je administrator naplate naloga koji će biti novi vlasnik za pretplatu, a zatim izaberite stavku pošalji **zahtev za prenos**
- Korisnik dobija e-poruku sa uputstvima da pregleda vaš zahtev za prenos. Da bi odobrio zahtev za prenos, korisnik odabira vezu u e-poruci i prati uputstva.

Natpis: Ako prebacite vlasništvo nad pretplatom na korisnički nalog u drugom Azure AD zakupcu, sve dodele kontrole pristupa [(RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) zasnovane na ulozi za upravljanje resursima u pretplati trajno se uklanjaju. Samo će novi vlasnik imati pristup za upravljanje resursima u pretplati. Više informacija potražite u [temi Prenos pretplate korisniku u drugom Azure AD zakupca.](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)

**Prenos vlasništva nad pretplatom**

Prenos vlasništva nad pretplatom preduslovi za pristup (RBAC) za upravljanje resursima u pretplati gube pristup. Više informacija o dodavanju postojeće pretplate u zakupca potražite u temi Povezivanje ili dodavanje [Azure pretplate](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)na Azure Active Directory.

- Prenos pretplate sa postojećim neizmećenim iznosom iz trenutnog ciklusa naplate neće biti prenet u novi instrument plaćanja u novom nalogu. Jedine informacije dostupne korisnicima u novom nalogu su cena pretplate za poslednji mesec. Ostatak istorije korišćenje i naplate ne prenosi se sa pretplatom.
- Vlasništvo nad prenosom ugovor za preduzeća (EA) pretplata trenutno je podržano samo na ugovor za preduzeća Portalu
- Prenos pretplate orijentisane na kredit kao što su Visual Studio, BizSpark, Microsoft Partner Network na novog korisnika zahteva da imate Visual Studio/Microsoft partnersku mrežnu licencu da biste prihvatili zahtev za prenos
- Svi resursi, kao što su virtuelne mašine, diskovi i veb sajtovi, uspešno se prenose na novi nalog. Prenos pretplate na više zakupca može da utiče na sledeće resurse:

**Azure AD usluge domena**

Trezori tastera Azure

- [SQL uticaj mogu da utiču](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) srodni korisnici i baze podataka, posebno ako klijent koristi Azure Active Directory povezanu potvrdu identiteta
- **Može da utiče** na usluge aplikacije konfigurisane Azure Active Directory potvrde identiteta
- **Visual Studio Tim** Nalozi usluga povezani sa Azure pretplatama mogu privremeno da izgube pristup kada se povezana Azure pretplata otkaže

**Preporučeni dokumenti**

Koraci nakon prihvatanja vlasništva nad naplatom:

- Da biste zadržali vlasništvo nad naplatom, ali promenili tip pretplate, pogledajte: Prebacite [Azure pretplatu na drugu ponudu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Prenos pretplata za projektante/testiranje za Visual Studio, Microsoft Partner Network (MPN) i Plaćanje po utrošku](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Prenos vlasništva nad naplatom ugovor za preduzeća (EA) pretplatama](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Prenos vlasništva – najčešća pitanja](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Rešavanje problema u vezi sa prenosom vlasništva](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)