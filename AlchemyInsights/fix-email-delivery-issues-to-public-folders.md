---
title: Rešavanje problema sa isporukom e-pošte u javne fascikle sa omogućenom poštom
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677942"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rešavanje problema sa isporukom e-pošte u javne fascikle sa omogućenom poštom

Ako spoljni pošiljaoci ne mogu da šalju poruke u javne fascikle sa omogućenom poštom pošte, a pošiljaoci imaju grešku: **nije bilo moguće pronaći (550 5.4.1)**, proverite da li je domen e-pošte za javnu fasciklu konfigurisan kao unutrašnji domen relej umesto autoritativno domen:

1. Otvorite [Exchange centar administracije (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Idite na **protok pošte** \> **prihvaćeni**domeni, izaberite prihvaćeni domen, a zatim kliknite na dugme **Uredi**.

3. Na stranici "Svojstva" koja se otvara, ako je tip domena podešen na **autoritativno**, promenite vrednost u **unutrašnji relej** , a zatim kliknite na dugme **Sačuvaj**.

Ako spoljni pošiljaoci dobiju grešku **nemate dozvolu (550 5.7.13)**, uradite sledeće komande u [Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste videli dozvole za anonimne korisnike u javnoj fascikli:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na primer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Da biste dopustili spoljnim korisnicima da šalju e-poštu u ovu javnu fasciklu, dodajte dugme Createstavke pravo na anonimni korisnik. Na primer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
