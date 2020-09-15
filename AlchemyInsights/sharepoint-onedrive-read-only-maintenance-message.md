---
title: Samo za čitanje kada pokušate da koristite SharePoint ili OneDrive
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
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670846"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Samo za čitanje kada pokušate da koristite SharePoint ili OneDrive

Korisnici mogu primati poruku **o održavanju samo za čitanje** kada pokušaju da koriste SharePoint ili OneDrive za neki od sledećih scenarija. 

-   Planirana ili aktivna aktivnost održavanja.  Potražite ih tako što ćete se u [centru za poruke](https://portal.office.com/adminportal/home#/messagecenter).
-   Događaj visokog prioriteta, aktivni servisni problem koji se možda dešava. Provjerite da li postoje savjeri/incidenti tako što ćete se usmeriti na [uslugu usluge](https://portal.office.com/adminportal/home#/servicehealth).
-   Međuverski scenario oporavka koji se može dogoditi zbog bilo kog neočekivanog događaja na serverima koji bi mogli da traju manje od 30 minuta ili tako nesto. 
    
    Ne postoje centar za poruke ili zdravstvene objave usluge za ova mala oporavka, ali trebalo bi da se brzo vratite u normalu.

U vrlo nekoliko navrata primećeni smo da je jedan od tri scenarija navedena u navedenom delu i da je usluga vraćena u prethodno stanje, ali keš korisnika pregledača nije očistljen.

Pokušajte da obrišite keš pregledača pre nego što se vratite na stranicu.

1. U Microsoft pregledaču Edge izaberite stavku **Postavke**, a zatim izaberite stavku **privatnost i bezbednost**.
2. U okviru **Izbriši pregledanje**izaberite **stavku odaberite šta da obrišete**.
3. Izaberite stavku **kolačići i sačuvani podaci o Veb lokaciji**i izaberite stavku **čisti**.

>[!Note] 
> Ovi koraci mogu da se razlikuju kada koristite druge pregledače kao što je Mozilla Firefox ili Google Chrome.

>[!Note] 
> Druga opcija bi bila da otvorite SharePoint sajt ili OneDrive u novom InPrivate prozoru.