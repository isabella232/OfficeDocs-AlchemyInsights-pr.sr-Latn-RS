---
title: Exchange PowerShell i osnovna zastarela potvrda identiteta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813486"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell i osnovna zastarela potvrda identiteta

Najnovije informacije o tome kako da se povežete sa uslugom Exchange Online PowerShell bez upotrebe osnovne potvrde identiteta [potražite ovde](https://aka.ms/exops-docs). Modul PowerShell V2 ne koristi osnovnu potvrdu identiteta.

Imajte u vidu da Osnovna potvrda identiteta i dalje mora da bude omogućena na klijentskom računaru.
Novi modul programa PowerShell v2 koristi modernu potvrdu identiteta za uspostavljanje veze za omogućavanje svih V2 cmdlet zasnovanih na REST. Pored V2 cmdlets, omogućava vam i da pristupate starijim daljinskim PowerShell (RPS) Cmdlets koje zahtevaju daljinsku PowerShell sesiju da bude uspostavljena. Uspostavljanje RPS sesije na Windows računaru zahteva da WinRM osnovna potvrda identiteta bude omogućena na računaru klijenta iako modul koristi mehanizam moderne potvrde identiteta za potvrdu identiteta usluge. WinRM kanal osnovne potvrde identiteta se koristi za prenošenje tokena moderne potvrde identiteta. Ako se WinRM kanal osnovne potvrde identiteta onemogući na računaru klijenta, novi V2 cmdlet nastaviće da radi (ali stariji RPS cmdlets neće).
