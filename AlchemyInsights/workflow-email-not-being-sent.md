---
title: E-pošta toka posla se ne šalje
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749003"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-pošta toka posla se ne šalje za SharePoint listu ili biblioteku

1. E-pošta iz tokova posla se ne šalju svim korisnicima ili samo određenim korisnicima ili vidite grešku **koju e-poruka nije moguće poslati. Proverite da li e-pošta ima važeće primaoca**.

    Potvrdite izbor u polju za proveru da li korisnik postoji u grupi dozvole za **sve osobe** (Lista korisničkih informacija) za tu kolekciju lokacija.  Uzorak direktnog URL adrese: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/ljudi Le.aspx? Članstvo "Grupito = 0

    - Ako korisnik ne postoji, uverite se da je korisnik prijavljen na stranicu. 
    - Ako je to spoljni korisnik, proverite da li je poziv prihvaжen.
    - Ako korisnik postoji u grupi dozvole, uverite se da je e-adresa tačna.
    - Ako adresa e-pošte korisnika nije postavljena ovde, kreirajte uzorak obaveštenja za tog korisnika koji obavezuje sinhronizaciju tog korisničkog naloga iz korisničkih profila sistema SharePoint u ovu kolekciju lokacija.
 
2. E-pošta iz tokova posla se šalje administratorima kolekcije lokacija, ali ne drugim korisnicima i pogledajte grešku **http zabranjenom na <span>https:</span>2016 url/_vti_bin/Client.XVC.SP.Utilities.Utility.sendemail**.
 

    [Pristup nije dozvoljen prilikom slanja e-poruke SharePoint grupi](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Pored toga, proverite da li funkcija za ograničenje kolekcije lokacija **ograničene pristupa korisniku** nije aktivna.


## <a name="related-topics"></a>Сродне теме
Želite da probate Microsoft flow u usluzi SharePoint online?
- [Kreiranje protoka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i protok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


