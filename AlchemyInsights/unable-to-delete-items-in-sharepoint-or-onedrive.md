---
title: Nije moguće izbrisati stavke u SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038531"
---
# <a name="unable-to-delete-items"></a>Nije moguće izbrisati stavke

- Smernice za zadržavanje mogu da do toga dospeju, morate da onemogućite ili isključite zadržavanje koje izaziva ovaj problem. Kada se smernice za zadržavanje ili zadržavanje uklone, može potrajati i do 24 časa dok promena ne stupi na snagu. Uverite se da za stavku [ne postoji podešavanje smernica](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) za zadržavanje.

- Lokacija je možda premašila ograničenje skladišta, povećala [kvotu lokacije](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i izbrisali stavku.

- Uverite se da stavka nije [odjavena](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugom korisniku.

- Na kraju, administratori [mogu da koriste SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) obrasce i prakse (PnP) koja sadrži biblioteku PowerShell komandi koje vam omogućavaju da izvršite složene radnje upravljanja kao što je nametnuto brisanje odsečaka stavki.
- [Uklanjanje PNP datoteke](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Uklanjanje PNP fascikle](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Uklanjanje stavke PNP liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Uklanjanje PNP liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Uklanjanje PNP polja (kolone)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)