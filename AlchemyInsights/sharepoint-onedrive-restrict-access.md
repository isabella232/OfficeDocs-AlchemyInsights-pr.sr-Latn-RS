---
title: Ograničavanje pristupa SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093855"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa SharePoint ili OneDrive

Postoji mnogo načina za ograničavanje pristupa SharePoint Online/OneDrive uslugama. Ovi različiti metodi ograničenja pristupa su podvučeni u nastavku. 

**Ograničenje dozvola**

U SharePoint online i OneDrive for Business, ograničavamo pristup stavkama kao što su lokacije, datoteke i fascikle samo tako što ćemo tim grupama/pojedincima koji treba da imaju pristup ograničavamo pristup.

- [Prilagođavanje dozvola za listu SharePoint biblioteku](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagođavanje SharePoint za lokaciju](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Promena dozvola za potfasciklu](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrola pristupa sa nekontrolišućeg uređaja](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kao SharePoint ili globalni administart, možete da blokirate ili ograničite pristup SharePoint i OneDrive sadržaju sa nekonvencijalih uređaja (oni koji nisu hibridni AD pridruženi ili usavršeni u aplikaciji Intune).

**Ograničenje mrežne lokacije**

Kao IT administrator možete da kontrolišete pristup resursima SharePoint i OneDrive na osnovu definisanih mrežnih lokacija u koje imate poverenja. Ovo je poznato i kao smernice zasnovane na lokaciji. Dodatne informacije potražite u [temi Kontrolisanje pristupa podacima SharePoint mreži i OneDrive podataka na osnovu mrežne lokacije](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograničenje zaključavanje lokacije** 

U SharePoint mreži imate mogućnost da zaključate kolekciju lokacija, tako da niko nema pristup. Ovo se postavlja putem programa PowerShell i [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću [svojstva Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**Ograničavanje korisnika da prave sajtove ili podsajtove**

Kao SharePoint ili globalni administarter, možete da omogućite korisnicima da kreiraju sopstvene SharePoint sajtove i administartuju ih, odrede koje vrste sajtova mogu da kreiraju i da navedu lokaciju sajtova. Dodatne informacije potražite u temi [Upravljanje kreiranjem sajta u SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

