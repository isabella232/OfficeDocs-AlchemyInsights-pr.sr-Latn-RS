---
title: Nadgledanje uslovnog pristupa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428313"
---
# <a name="monitor-intune-conditional-access"></a>Nadgledanje uslovnog pristupa

Korisnici koji su usmereni na uslovno pristup dobiće obaveštenje ako ne ispune zahteve za pristup vaše organizacije. Da biste rešili, preporučujemo neka od sledećih rešenja:

1. Ako se na uređaj pretpostavlja da je upisan, savetujte korisnika da ode na aplikaciju portala preduzeća i potvrdi da se pojavljuje na portalu preduzeća. Ako nije, korisnik mora da prijavi uređaj.
1. U Azure portalu **Idite na**  >  **usaglašenost uređaja**. 
1. Da biste videli izveštaj o usaglašenosti uređaja da biste proverili da li je uređaj za korisnike označen kao usaglašeni, u okviru **monitor** izaberite stavku **usaglašenost uređaja**.
1. U Azure portalu **Idite na**  >  **usaglašenost uređaja**. U okviru **Upravljanje** izaberite stavku **smernice**. Na listi smernica usaglašenosti proverite da li je profil dodeljen vašem uređaju. Ako nijedan profil nije dodeljen, Intune neće moći da potvrdi status usaglašenosti uređaja.
1. Uredite zadatak korisnika uslovnog pristupa.
1. Na Azure portalu idite da biste **podesili**  >  **uslovne**  >  **smernice** za pristup, izaberite smernice sa liste i izaberite stavku **korisnici i grupe**.
1. Da biste nekome ciljali određenu politiku, dodajte ih na **listu "ukljuci**". Da biste se uverili da je osoba izostavljena iz smernica, dodajte ih na **listu "Isključi**".

**Korisne veze:**

- [Pregled usaglašenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Rešavanje problema sa kom](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Smernice za rešavanje problema](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Nadgledanje usaglašenosti uređaja](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Ovi koraci su korisni samo u rešavanju problema sa funkcijom Azure Active Directory. Uređaj može da blokira i blokiranje pristupa e-poštom pomoću Exchange smernica. Više informacija o upravljanju Exchange uređajima možete da pronađete [**ovde**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
