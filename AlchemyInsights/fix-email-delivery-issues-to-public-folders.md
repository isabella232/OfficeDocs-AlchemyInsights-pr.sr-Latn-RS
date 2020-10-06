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
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366478"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rešavanje problema sa isporukom e-pošte u javne fascikle sa omogućenom poštom

Ako spoljni pošiljaoci ne mogu da šalju poruke u javne fascikle sa omogućenom poštom pošte, a pošiljaoci imaju grešku: **nije bilo moguće pronaći (550 5.4.1)**, proverite da li je domen e-pošte za javnu fasciklu konfigurisan kao unutrašnji domen relej umesto autoritativno domen:

1. Otvorite [Exchange centar administracije (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Idite na **protok pošte** \> **prihvaćeni**domeni, izaberite prihvaćeni domen, a zatim kliknite na dugme **Uredi**.

3. Na stranici "Svojstva" koja se otvara, ako je tip domena podešen na **autoritativno**, promenite vrednost u **unutrašnji relej** , a zatim kliknite na dugme **Sačuvaj**.

Ako spoljni pošiljaoci dobiju grešku **nemate dozvolu (550 5.7.13)**, uradite sledeće komande u [Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste videli dozvole za anonimne korisnike u javnoj fascikli:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na primer, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Da biste dopustili spoljnim korisnicima da šalju e-poštu u ovu javnu fasciklu, dodajte dugme Createstavke pravo na anonimni korisnik. Na primer, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
