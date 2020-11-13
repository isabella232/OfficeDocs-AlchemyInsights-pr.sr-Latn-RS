---
title: Nije moguće izbrisati stavke u sistemu SharePoint ili OneDrive
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
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019597"
---
# <a name="unable-to-delete-items"></a>Nije moguće izbrisati stavke

- Smernice za zadržavanje mogu uzrokovati ovu grešku, treba da onemogućite ili isključite odgovarajući čekanje koji uzrokuje ovaj problem. Kada se ukloni polisa za zadržavanje ili čekanje, može biti potrebno do 24 časa da bi promena stupila na snagu. Uverite se da nije podešena [smernica za zadržavanje](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) za stavku.

- Lokacija je možda premašila ograničenje skladišta, povećavanje [kvote](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) i brisanje stavke.

- Uverite se da stavka nije [odjavljena](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) na drugog korisnika.

- Konačno, administratori mogu da koriste [SharePoint obrasce i prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) koji sadrže biblioteku PowerShell komandi koje vam omogućava da obavljate komplikovane radnje upravljanja kao što je prinudno brisanje tvrdoglavih stavki.
- [Ukloni PNP datoteku](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [Uklanjanje PNP fascikle](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [Uklanjanje stavke PNP liste](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [Ukloni PNP listu](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [Uklanjanje PNP polja (kolona)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)