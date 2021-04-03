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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505703"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Vraćanje izbrisane Microsoft 365 grupe

Možete da vratite izbrisanu Microsoft 365 grupu ili Microsoft Teams u roku od 30 dana od brisanja.

1. Da biste se prijavili u Microsoft 365 centar adminizbrišete i naveli izbrisane grupe i timove, idite u [Microsoft 365 centar za administaciju.](https://aka.ms/RestoreDeletedGroup)

    **Napomogućeno:** Prijavite se pomoću naloga koji je dodeljen administratoru zakupca ili ulozi administratora grupe.

1. Izaberite izbrisanu Microsoft 365 grupu/Teams za vraćanje u prethodno stanje i kliknite na vrati **grupu.**

    Ako nije moguće vratiti grupu zbog neusaglašene SMTP adrese, koristite sledeću komandu da biste pronašli objekat koji izaziva neusaglašenost i uklonili SMTP adresu:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Napomogućeno:** U nekim slučajevima može biti čak do 24 časa da grupe i svi njeni podaci budu vraćeni u prethodno stanje.

    Dodatne informacije ili da biste saznali kako da vratite grupe u prethodno stanje pomoću programa PowerShell potražite u članku Vraćanje [izbrisane Microsoft 365 grupe.](https://go.microsoft.com/fwlink/?linkid=867802)