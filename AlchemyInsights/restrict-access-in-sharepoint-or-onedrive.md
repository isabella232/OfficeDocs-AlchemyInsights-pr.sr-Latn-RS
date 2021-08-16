---
title: Ograničavanje pristupa SharePoint ili OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075054"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa SharePoint ili OneDrive

U SharePoint i OneDrive, ograničavate pristup stavkama kao što su datoteke, fascikle i liste tako što dodeljute pristup samo grupama ili pojedincima za koje želite da imaju pristup. Dozvole u programu SharePoint su podrazumevano nasleđene od viših nivoa u hijerarhiji. Tako datoteka nasleđuje dozvole od fascikle, koja nasleđuje dozvole od biblioteke, koja nasleđuje dozvole od lokacije.
  
Možete da delite na višem nivou (na primer, deljenjem cele lokacije), a zatim prekinete nasleđivanje ako ne želite da delite sve stavke na lokaciji. Međutim, to ne preporučujemo jer čini održavanje dozvola složenijim i zbunjujućim u budućnosti. Evo šta možete da uradite umesto toga:
  
- Na primer, ako želite da delite sav sadržaj fascikle osim jedne datoteke u kojoj se nalazi, premestite tu datoteku na novu lokaciju koja se ne deli.
    
- Ako imate dve potfascikle u fascikli i želite da delite jednu potfasciklu sa grupama A i B i dozvolite samo grupi A pristup drugoj potfascikli, delite nadređenu fasciklu sa grupom A i dodajte grupu B u prvu potfasciklu.
    
[Zaustavljanje deljenja datoteke ili fascikle ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

