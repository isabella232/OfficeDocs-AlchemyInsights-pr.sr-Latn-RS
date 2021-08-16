---
title: Rešavanje problema sa isporukom e-pošte u javne fascikle omogućene za poštu
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
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068826"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Rešavanje problema sa isporukom e-pošte u javne fascikle omogućene za poštu

Ako spoljni pošiljalac ne može da pošalje poruke u javne fascikle pošte, a pošiljalac dobija grešku: nije moguće pronaći **(550 5.4.1),** proverite da li je domen e-pošte javne fascikle konfigurisan kao interni relejni domen umesto ovlašćenog domena:

1. Otvorite [Exchange za administaciju (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Idite na **Prihvaćeni** \> **domeni pošte**, izaberite prihvaćeni domen, a zatim kliknite na dugme **Uredi**.

3. Na stranici sa svojstvima koja se otvori, ako je tip domena postavljen na "Ovlašćeno", promenite vrednost u Interni **relej,** a zatim kliknite na dugme **Sačuvaj**.

Ako spoljni pošiljalac dobije grešku da nemate dozvolu **(550 5.7.13),** pokrenite sledeću komandu u programu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) da biste videli dozvole za anonimne korisnike u javnoj fascikli:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Na `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` primer, .

Da biste spoljnim korisnicima dozvolili da šalju e-poštu u ovu javnu fasciklu, dodajte pristup CreateItems odmah korisniku Anonimno. Na `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` primer, .
