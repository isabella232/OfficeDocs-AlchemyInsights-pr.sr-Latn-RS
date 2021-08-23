---
title: Postavka Outlook oznake nije primenjena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/17/2021
ms.locfileid: "58455088"
---
# <a name="default-outlook-label-setting-not-applied"></a>Postavka Outlook oznake nije primenjena

Ako se Outlook podrazumevane postavke nalepnice ne primenjuju ispravno i ako se primenjuju druge oznake ili nije primenjena nijedna nalepnica, možda imate poznat problem (MC277818) i treba da uradite nešto od ove 2 opcije da biste rešili problem:

**1. opcija:**

1. Idite u Microsoft 365 centra za usaglašenost i >   >  **Information Protection za rešenja.**
1. Izaberite **Smernice za nalepnice**, a zatim izaberite smernice za nalepnice koje treba da uredite (**OutlookDefaultlabel** postavka nije ispravno postavljena na datoj smernici nalepnica. Pokrenite **Get-labelpolicy da** biste prikazali ovu postavku), a zatim izaberite stavku **Uredi smernice**.
1. Kliknite na **dugme** Dalje dok ne vidite postavku Primeni ovu  podrazumevanu nalepnicu na e-poruke **,**  koja je dostupna ako izaberete opciju Zahtevaj od korisnika da primene nalepnicu na e-poruke i dokumente sa oznakom "heš" u dijalogu Postavke smernica.
1. U **dijalogu Primena podrazumevane oznake na dokumente** sa **padajuće** liste odaberite stavku Nijedno.
1. Kliknite na **dugme Dalje** **i Prosledi** da biste sačuvali postavke nalepnice.

**2. opcija:**

U [powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)centru za bezbednost i usaglašenost koristite komandu "Set-LabelPolicy" da biste promenili **komandu OutlookDefaultlabel** u **Nijedno** na {OutlookDefaultLabel="None"}.

Pokreni: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Dodatne informacije o podrazumevanim nalepnicama za Outlook potražite u temi Podešavanje druge [podrazumevane nalepnice za Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)