---
title: Čuvanje lokacije ili liste kao predloška
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109218"
---
# <a name="save-site-or-list-as-a-template"></a>Čuvanje lokacije ili liste kao predloška

SharePoint lokacija su unapred izbuđene definicije dizajnirane za određenu poslovnu potrebu. Više informacija potražite u [temi Korišćenje predložaka za pravljenje različitih vrsta SharePoint lokacija.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Ovo su neki uobičajeni problemi/rešenja u vezi sa čuvanjem lokacije ili liste kao predloška u SharePoint Online.

**Dugme "Sačuvaj lokaciju/predložak liste" nije dostupno ili nedostaje**. 

- Administratori će morati da dozvole prilagođenu skriptu da bi omogućili funkcije predloška. Detaljne korake, primere i stavke koje treba razmotriti možete da vidite u temi [Dozvoljavanje ili sprečavanje prilagođene skripte.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Komanda Sačuvaj lokaciju kao predložak nije podržana i može da izazove probleme na lokacijama koje koriste infrastrukturu SharePoint servera za objavljivanje.


**Nije moguće kreirati predložak lokacije ili ne funkcioniše ispravno**

- Moguće je da predlošku nedostaje [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće da se aktivira. Ako funkcija nije dostupna za aktivaciju u trenutnoj kolekciji lokacija, ne možete koristiti predložak lokacije za kreiranje lokacije.


- Proverite da li neka lista ili [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) biblioteka premašuje ograničenje prikaza liste od 5000 stavki, što može blokirati kreiranje predloška lokacije.


- Lokacija možda koristi previše resursa, stoga predložak lokacije premašuje ograničenje od 50 megabajta (MB).


- Postoje problemi u prikazivanje podataka sa liste koja koristi kolonu za pronalaženje. Više informacija potražite u temi Lista koja je generisana predloškom ne prikazuje podatke sa ispravne liste za pronalaženje [u programu SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Detaljnije informacije o uobičajenim problemima i rešenjima potražite u temi Kreiranje [i korišćenje predložaka lokacije.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

