---
title: Izvoz rezultata pretrage eDiscovery/otkrivanja sadržaja
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429971"
---
# <a name="export-ediscoverycontent-search-results"></a>Izvoz rezultata pretrage eDiscovery/otkrivanja sadržaja

Možda ćete morati da izvezete rezultate pretrage u PST datoteku (iz e-pošte) ili u izvorne Office dokumente (iz sistema SharePoint i usluge OneDrive for Business sites). Ako je tako, uradite sledeće:

- Uverite se da je nalogu dodeljen odgovarajući pristup za izvoz. Više informacija potražite u članku [dodeljivanje dozvole za eDiscovery](https://go.microsoft.com/fwlink/?linkid=2102406).
- Uverite se da je računar ispunio sve [preduslove](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin). Nisu podržani svi pregledači, kao što je Chrome.
- Da biste izvezli iz pretrage sadržaja: a. Idite u [Centar za bezbednost & bezbednosti](https://protection.office.com/contentsearch) i kliknite na dugme **Pretraži**, a zatim izaberite stavku **Pretraga sadržaja**. Na stranici **Pretraga sadržaja** izaberite sačuvanu pretragu.
    -. U oknu detalji, u okviru **Izvezi rezultate na računar**, izaberite stavku **Započni izvoz**. Ako izvozite više od 100K poštanskih sandučića, moraćete da koristite PowerShell da biste preuzeli rezultate izvoza. Više informacija potražite u članku [izvoz rezultata iz više od 100K poštanskih sandučića](https://go.microsoft.com/fwlink/?linkid=2143861).

Da biste saznali više, pogledajte članak [izvoz rezultata pretrage sadržaja](https://go.microsoft.com/fwlink/?linkid=2102118).