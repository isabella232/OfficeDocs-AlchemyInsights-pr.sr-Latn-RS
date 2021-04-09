---
title: Vraćanje izbrisane Microsoft 365 grupe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645145"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Vraćanje izbrisane Microsoft 365 grupe

Možete da vratite izbrisanu Microsoft 365 grupu ili Microsoft Teams u roku od 30 dana od brisanja.

1. Idite u [Microsoft 365](https://aka.ms/RestoreDeletedGroup) centar za administaciju da biste se prijavili na listu izbrisanih grupa i timova.

    **Napomogućeno:** Prijavite se pomoću naloga koji je dodeljen administratoru zakupca ili ulozi administratora grupe.

1. Izaberite izbrisanu Microsoft 365 grupu/Teams za vraćanje u prethodno stanje i kliknite na vrati **grupu.**

    Ako nije moguće vratiti grupu zbog neusaglašene SMTP adrese, koristite sledeću komandu da biste pronašli objekat koji izaziva neusaglašenost i uklonili SMTP adresu:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Napomogućeno:** U nekim slučajevima može biti čak do 24 časa da grupe i svi njeni podaci budu vraćeni u prethodno stanje.

    Dodatne informacije ili da biste saznali kako da vratite grupe u prethodno stanje pomoću programa PowerShell potražite u članku Vraćanje [izbrisane Microsoft 365 grupe.](https://go.microsoft.com/fwlink/?linkid=867802)