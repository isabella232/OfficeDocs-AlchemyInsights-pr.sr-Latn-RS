---
title: Više korisnika preuzimanje greške zabrane pristupa pri dodavanju programskih dodataka u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424173"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Više korisnika preuzimanje greške zabrane pristupa pri dodavanju programskih dodataka u programu Outlook

Možete da navedete koje administratori u vašoj organizaciji imaju dozvolu da instaliraju i upravljaju programskim dodacima za Outlook. Takođe možete odrediti koji korisnici u vašoj organizaciji imaju dozvolu da instaliraju i upravljaju programskim dodacima za svoje korišćenje.

Više informacija potražite u članku [Određivanje administratora i korisnika koji mogu da instaliraju i upravljaju programskim dodacima za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Da biste proverili da li ste uspešno dodelili dozvole za korisnika, zamenite <Role Name> ime uloge koju želite da proverite i pokrenite sledeću komandu u Exchange online PowerShell:

Preuzimanje-uloga " <Role Name> "-GetEffectiveUsers

Ovaj primer vam pokazuje kako da proverite kome ste dodelili dozvole za instaliranje programskih dodataka iz Office prodavnice za organizaciju.

PowerShell

-Uloga "aplikacije Marketplace org"-GetEffectiveUsers

U rezultatima, preuzmi i ponovo dodeli, Pregledajte stavke u koloni "efektivni korisnici".

Za detaljne informacije o sintaksi i parametrima pogledajte odeljak preuzimanje obaveštenja o [dodelju](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 