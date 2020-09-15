---
title: Ograničavanje pristupa u sistemu SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700469"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Ograničavanje pristupa u sistemu SharePoint ili OneDrive

Postoji mnogo načina za ograničavanje pristupa na SharePoint online/OneDrive uslugama. Ovi različiti metodi ograničenja pristupa su naglašeni ispod. 

**Ograničenje dozvole**

U sistemu SharePoint Online i OneDrive for Business ograničavamo pristup stavkama kao što su lokacije, datoteke i fascikle tako što omogućavamo samo pristup tim grupama/osobama koje treba da imaju pristup.

- [Prilagođavanje dozvola za SharePoint listu ili biblioteku](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [Prilagođavanje dozvola za SharePoint sajt](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [Promena dozvola u potfascikli](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [Kontrola pristupa iz nekompletnih uređaja](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

Kao SharePoint ili globalni administrator, možete da blokirate ili ograničite pristup SharePoint i OneDrive sadržaju iz nekompletnih uređaja (oni koji nisu hibridni oglas spojeni u Intune).

**Ograničenje mrežne lokacije**

Kao IT administrator, možete da kontrolišete pristup SharePoint i OneDrive resursima na osnovu definisanih mrežnih lokacija u koje imate poverenja. Ovo je takođe poznato kao smernice zasnovane na lokaciji. Više informacija potražite u članku [Kontrola pristup SharePoint Online i OneDrive podacima na osnovu mrežne lokacije](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**Ograničenje zaključavanje lokacija** 

U sistemu SharePoint online imate mogućnost da zaključate kolekciju lokacija, tako da niko nema pristup. Ovo je podešeno putem programskog dodatka PowerShell i [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) pomoću nekretnina [seta-sposite-](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) lockstate.

**Ograničavanje korisnika da kreiraju lokacije ili podlokacije**

Kao SharePoint administrator ili globalni administrator, možete da omogućite korisnicima da kreiraju i upravljaju sopstvenim SharePoint lokacijama, odrede koje lokacije mogu da kreiraju i navode lokaciju lokacija. Više informacija potražite [u članku Upravljanje kreiranjem lokacije u usluzi SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)

