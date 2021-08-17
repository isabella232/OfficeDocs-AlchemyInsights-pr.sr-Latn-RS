---
title: Kreiranje sajta u programu SharePoint Online
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057980"
---
# <a name="create-sharepoint-sites-using-templates"></a>Kreiranje SharePoint sajtova pomoću predložaka

Mogućnost čuvanja lokacije kao predloška nije podržana uz modernu komunikaciju ili sajtove tima. Više informacija o korišćenju predložaka potražite u [temi Čuvanje, preuzimanje i otpremanje SharePoint lokaciji kao predloška.](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

Ovo su neki uobičajeni problemi/rešenja u vezi sa čuvanjem lokacije ili liste kao predloška u programu SharePoint Online. 

**Dugme "Sačuvaj lokaciju/predložak liste" nije dostupno ili nedostaje**

Administratori će morati da dozvole prilagođenu skriptu da bi omogućili funkcije predloška. Detaljne korake, primere i razmatranja pogledajte u temi 

- [Dozvoljavanje ili sprečavanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Komanda Sačuvaj lokaciju kao predložak nije podržana i može da izazove probleme na lokacijama koje koriste infrastrukturu SharePoint servera za objavljivanje.

**Nije moguće kreirati predložak lokacije ili ne funkcioniše ispravno**

Moguće je da predlošku nedostaje [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće da se aktivira. Ako funkcija nije dostupna za aktivaciju u trenutnoj kolekciji lokacija, ne možete koristiti predložak lokacije za kreiranje lokacije.

- Proverite da li neka lista ili [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) biblioteka premašuje ograničenje prikaza liste od 5000 stavki, što može blokirati kreiranje predloška lokacije.

- Lokacija možda koristi previše resursa, stoga predložak lokacije premašuje ograničenje od 50 MB.


- Postoje problemi u prikazivanje podataka sa liste koja koristi kolonu za pronalaženje. Više informacija potražite u temi Lista koja je generisana predloškom ne prikazuje podatke sa ispravne liste za pronalaženje [u programu SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)

Detaljnije informacije o uobičajenim problemima i rešenjima potražite u temi Kreiranje i [korišćenje predložaka lokacije.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



