---
title: Čuvanje stranice ili liste kao predloška
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727545"
---
# <a name="save-site-or-list-as-a-template"></a>Čuvanje stranice ili liste kao predloška

Predlošci SharePoint lokacije su unapred izgrađeni definicijedizajnirani oko određenih poslovnih potreba. Više informacija potražite u članku [Korišćenje predložaka za kreiranje raznih vrsta SharePoint lokacija](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Evo nekih uobičajenih problema/rešenja u vezi sa čuvanjem lokacije ili liste kao predloška u usluzi SharePoint online.

**Dugme "Sačuvaj predložak sajta/liste" nije dostupno ili nedostaje**. 

- Administratori će morati da dozvole prilagođenu skripcu za omogućavanje funkcija predloška. Detaljniji koraci, primeri i problemi vide [Omogućavanje ili sprečavanje prilagođenog skriptova](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Komanda "Sačuvaj lokaciju kao predložak" nije podržana i može da izazove probleme na lokacijama koje koriste infrastrukturu za objavljivanje na SharePoint serveru.


**Nije moguće kreirati predložak veb sajta ili ne funkcioniše ispravno**

- Predlošku možda nedostaje [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati. Ako funkcija nije dostupna za aktiviranje trenutne kolekcije lokacija, ne možete da koristite predložak Veb lokacija da biste kreirali sajt.


- Potvrdite izbor u ovom polju za proveru da li bilo koje liste ili biblioteke premašuju [cenzus](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 stavki pomoću kojih to može da blokira Kreiranje predloška sajta.


- Lokacija možda koristi previše resursa i samim tim, predložak sajta premašuje ograničenje od 50 megabajta (MB).


- Postoje problemi sa prikazivanjem podataka sa liste koja koristi kolonu za pronalaženje. Više informacija potražite u članku [lista sa obrascem koji je generisao ne pokazuje podatke sa odgovarajuće liste za pronalaženje u usluzi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Detaljnije informacije o uobičajenim problemima i rešenjima navedite, [Kreirajte i koristite predloške lokacija](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

