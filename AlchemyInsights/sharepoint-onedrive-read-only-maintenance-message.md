---
title: Read-Only za poruku "Održavanje" prilikom pokušaja korišćenja usluge SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329462"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only za poruku "Održavanje" prilikom pokušaja korišćenja usluge SharePoint ili OneDrive

Korisnici mogu da dobiju poruku samo za čitanje za **održavanje** kada pokušaju da koriste ovu SharePoint ili OneDrive za neki od sledećih scenarija. 

-   Planirana ili aktivna aktivna aktivna aktivnost održavanja.  Proverite da li ih ima tako što biste odšli u [centar za poruke.](https://portal.office.com/adminportal/home#/messagecenter)
-   Može da se desi aktivan incident sa aktivnom uslugom visokog prioriteta. Proverite savete/incidente tako što će odu do stavke [Zdravstveno stanje usluge.](https://portal.office.com/adminportal/home#/servicehealth)
-   Manji scenario oporavka od automatskog kašnjenja koji se može desiti usled bilo kakvih neočekivanih događaja na serverima koji mogu trajati manje od 30 minuta ili tako dalje. 
    
    Nema centra za poruke ili objava o stanju usluge za ove manje oporavke, ali bi uskoro trebalo da se vratite na normalan.

U nekoliko prilika smo primetili da je jedan od tri gorenavedena scenarija uzrok i usluga je vraćena u prethodno stanje, ali keš pregledača korisnika nije obrozan.

Pokušajte da obrrišete keš pregledača pre nego što odete na lokaciju.

1. U pregledaču Microsoft Edge izaberite stavku **Postavke**, a zatim izaberite privatnost **i bezbednost**.
2. U **okviru Stavke Obriši pregledanje** izaberite **stavku Odaberite stavke za brisanje**.
3. Izaberite **Kolačići i sačuvani podaci o veb lokacijama**, a zatim izaberite **stavku Obriši**.

**Napomena:** Ovi koraci mogu da se razlikuju kada koristite druge pregledače kao što su Mozilla Firefox ili Google Chrome.

**Napomi:** Druga opcija je da otvorite SharePoint lokaciju ili OneDrive u novom InPrivate prozoru.