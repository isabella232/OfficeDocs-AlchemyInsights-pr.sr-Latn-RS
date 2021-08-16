---
title: E-poruka toka posla se ne šalje
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072534"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-poruka toka posla se ne šalje za SharePoint listu ili biblioteku

1. E-pošta od tokova posla se ne šalje svim korisnicima ili samo određenim korisnicima ili vidite grešku E-poruka se ne može poslati. Uverite se da **e-poruka** ima važećog primaoca.

    Proverite da li korisnik postoji u grupi **dozvola "Sve osobe"** (na listi informacija o korisniku) za tu kolekciju lokacija.  Uzorak direktne URL adrese: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Ako korisnik ne postoji, proverite da li je korisnik prijavljen na stranicu. 
    - Ako je to spoljni korisnik, uverite se da je njegov poziv prihvaćen.
    - Ako korisnik postoji u grupi dozvola, proverite da li je e-adresa ispravna.
    - Ako e-adresa korisnika nije ovde postavljena, kreirajte uzorak obaveštenja za tog korisnika koji nameće sinhronizaciju tog korisničkog naloga sa korisničkih profila korisnika SharePoint sa ovom kolekcijom lokacija.
 
2. E-pošta od tokova poslata je administratorima kolekcije lokacija, ali ne drugim korisnicima i vide grešku HTTP zabranjeno **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Pogledajte [pristup odbijen kada pošaljete e-poruku SharePoint grupi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Proverite i da funkcija kolekcije lokacija **režima zaključavanja korisničke** dozvole ograničenog pristupa nije aktivna.


## <a name="related-topics"></a>Сродне теме
Želite da probate Microsoft Flow u SharePoint Online?
- [Kreiranje Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


