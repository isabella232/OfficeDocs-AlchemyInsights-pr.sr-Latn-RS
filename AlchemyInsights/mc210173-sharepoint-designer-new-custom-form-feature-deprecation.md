---
title: MC210173 – Novi prilagođeni obrazac zastarevanja funkcije SharePoint Designer programa
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
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831820"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 – Novi prilagođeni obrazac zastarevanja funkcije SharePoint Designer programa

Identifikovali smo problem koji utiče na funkcionalnost SharePoint Designer programa za [kreiranje prilagođenih obrazaca](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) unutar usluge SharePoint Online. Nakon pažljivog ispitivanja, utvrdili smo da ne postoji poznata ispravka za ovaj problem i odlučili smo da onemogućimo prilagođenu funkciju izrade obrasca koja će važiti od 3:00 UTC u subotu, 25. aprila 2020. Ova promena ne utiče na mogućnost uređivanja prethodno stvorenih obrasca ili drugih postojećih funkcija u SharePoint Online dizajneru.

Nakon što je ova promena izvršena, korisnici su možda dobili grešku: „Nije moguće sačuvati promene na listi servera“ prilikom kreiranja novih obrazaca.

Korisnici koji su prethodno koristili SharePoint Designer za kreiranje prilagođenih obrasca umesto toga mogu da iskoriste [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) u tu svrhu.

PowerApps je jednostavan i moćan alat koji omogućava korisnicima koji rade u SharePoint Online modernom iskustvu da kreiraju i uređuju prilagođene obrasce za SharePoint liste i biblioteke dokumenata direktno iz prozora pregledača. PowerApps ne zahteva tradicionalno znanje kodiranja ili bilo koje dodatno preuzimanje aplikacija kao što je InfoPath.

**Napomena**: SharePoint Online klasični korisnici moraće da se privremeno prebace na moderno iskustvo da bi pristupili PowerApps i koriste PowerApps. Međutim, svim prilagođenim obrascima koji su kreirani u PowerApps mogu da pristupe korisnici SharePoint Online klasičnog iskustva.
