---
title: Sadržaj se ne pojavljuje u SharePoint rezultatima pretrage
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713144"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Sadržaj se ne pojavljuje u SharePoint rezultatima pretrage

Slijedite ove korake za rešavanje problema kada se očekivani sadržaj ne pojavljuje u rezultatima pretrage:
  
1. Potvrdite da je **lokacija** koja sadrži očekivani sadržaj podešena da omogući da se sadržaj pojavi u rezultatima pretrage. Slijedite korake u programu [Prikaži sadržaj na sajtu u rezultatima pretrage](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Potvrdite da je **Lista** ili **Biblioteka** koja sadrži očekivani sadržaj podešena tako da omogući da se sadržaj pojavi u rezultatima pretrage. Slijedite korake u [članku prikazivanje sadržaja iz lista ili biblioteka u rezultatima pretrage](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Potvrdite da se stranica, dokument ili prilagođeni raspored na stranici objavljuje kao **glavna verzija.** Sledi treći broj u [tražanju ne vraća sve rezultate u usluzi SharePoint online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Proverite da li korisnik ima **dozvole** za prikaz sadržaja. Slijedite korake u [razumevanju nivoa dozvola u sistemu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Ako je šema pretrage promenjena tako što ćete dodati novo upravljano vlasništvo, uređivanjem upravljanog vlasništva ili uklanjanjem kontrolisanog polja, moraćete da zahtevate popisivanje i ponovno indeksiranje. **Ponovno indeksiranje** sadržaja tako što ćete pratiti korake u [ručno zahtevanje popisivanja i ponovno indeksiranje sajta, biblioteke ili liste](https://docs.microsoft.com/sharepoint/crawl-site-content). Ovo može potrajati, sačekati 24 časa pre nego što ponovo proveravate rezultate.

Više informacija potražite u članku [Omogućavanje pretraživanja sadržaja na sajtu](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
