---
title: Ograničavanje pristupa u sistemu SharePoint ili OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720696"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u sistemu SharePoint ili OneDrive

U sistemu SharePoint i OneDrive ograničite pristup stavkama kao što su datoteke, fascikle i liste tako što ćete dodeliti Access samo grupama ili osobama koje želite da imate. Dozvole u sistemu SharePoint podrazumevano su nasleđene iz većeg dodatka u hijerarhiji. Tako da datoteka nasleđuje svoje dozvole iz fascikle, koja nasleđuje dozvole iz biblioteke, koja nasleđuje dozvole od lokacije.
  
Možete da delite na većem nivou (na primer, tako što ćete deliti celu stranicu), a zatim prekinuti nasledstvo ako ne želite da delite sve stavke na lokaciji. Međutim, ovo ne preporučujemo zato što vam ubuduće omogućava da održavate dozvole složenije i zbunjujuće. Evo šta možete da uradite umesto toga:
  
- Ako, na primer, želite da delite celokupan sadržaj fascikle, osim za jednu datoteku, premestite tu datoteku na novu lokaciju koja se ne deli.
    
- Ako imate dve potfascikle u fascikli i želite da delite jednu potfasciklu sa grupama A i B i omogućite samo pristup grupi u drugu potfasciklu, delite nadređenu fasciklu sa grupom a i dodajte grupu B u prvu potfasciklu.
    
[Zaustavljanje deljenja datoteke ili fascikle ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

