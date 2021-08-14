---
title: Vraćanje izbrisane Microsoft 365 grupi
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959040"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Vraćanje izbrisane Microsoft 365 grupi

Izbrisanu grupu ili Microsoft 365 Microsoft Teams možete vratiti u prethodno stanje u roku od 30 dana od brisanja.

1. Idite na [Microsoft 365 centar administracije](https://aka.ms/RestoreDeletedGroup) da biste se prijavili na listu izbrisanih grupa i timova.

    **Napomogućeno:** Prijavite se pomoću naloga koji je dodeljen administratoru zakupca ili ulozi administratora grupe.

1. Izaberite izbrisane Microsoft 365 grupe/grupe/Teams da se vratite u prethodno stanje i izaberite stavku vrati **grupu u prethodno stanje.**

    Ako nije moguće vratiti grupu zbog neusaglašene SMTP adrese, koristite sledeću komandu da biste pronašli objekat koji izaziva neusaglašenost i uklonili SMTP adresu:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Napomogućeno:** U nekim slučajevima može biti čak do 24 časa da grupe i svi njeni podaci budu vraćeni u prethodno stanje.

    Dodatne informacije ili da biste saznali kako da vratite grupe u prethodno stanje pomoću programa PowerShell potražite u članku Vraćanje [izbrisane Microsoft 365 grupi.](https://go.microsoft.com/fwlink/?linkid=867802)