---
title: Kreiranje lokacije u usluzi SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732252"
---
# <a name="create-sharepoint-sites-using-templates"></a>Kreiranje SharePoint lokacija pomoću predložaka

Mogućnost čuvanja lokacije kao predloška nije podržana uz modernu komunikaciju ili lokacije tima. Više informacija o korišćenju predložaka potražite [u članku čuvanje i otpremanje SharePoint lokacije kao predloška](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Evo nekih uobičajenih problema/rešenja u vezi sa čuvanjem lokacije ili liste kao predloška u usluzi SharePoint online. 

**Dugme "Sačuvaj predložak sajta/liste" nije dostupno ili nedostaje**

Administratori će morati da dozvole prilagođenu skripcu za omogućavanje funkcija predloška. Detaljne korake, primeri i razmatranja 

- [Omogućavanje ili sprečavanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Komanda "Sačuvaj lokaciju kao predložak" nije podržana i može da izazove probleme na lokacijama koje koriste infrastrukturu za objavljivanje na SharePoint serveru.

**Nije moguće kreirati predložak veb sajta ili ne funkcioniše ispravno**

Predlošku možda nedostaje [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati. Ako funkcija nije dostupna za aktiviranje trenutne kolekcije lokacija, ne možete da koristite predložak Veb lokacija da biste kreirali sajt.

- Potvrdite izbor u ovom polju za proveru da li bilo koje liste ili biblioteke premašuju [cenzus](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 stavki pomoću kojih to može da blokira Kreiranje predloška sajta.

- Lokacija možda koristi previše resursa i samim tim, predložak sajta premašuje ograničenje od 50 MB.


- Postoje problemi sa prikazivanjem podataka sa liste koja koristi kolonu za pronalaženje. Više informacija potražite u članku [lista sa obrascem koji je generisao ne pokazuje podatke sa odgovarajuće liste za pronalaženje u usluzi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Detaljnije informacije o uobičajenim problemima i rešenjima potražite u okviru [Kreiranje i korišćenje predložaka lokacija](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



