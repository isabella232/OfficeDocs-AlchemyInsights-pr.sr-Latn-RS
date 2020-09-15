---
title: Kako da onemogućite spoljne grupe
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704142"
---
# <a name="how-to-disable-external-groups"></a>Kako da onemogućite spoljne grupe

Yammer spoljna razmena poruka primenjuje Exchange pravila transporta (ETRs), skupa proaktivnih kontrola radi sprečavanja deljenja informacija o preduzeću. Da biste ograničili korisnike da kreiraju spoljne grupe, treba da konfigurišete pravilo za razmenu Exchange servera (ETR), a zatim da konfigurišete Yammer da koristi pravilo Exchange transporta za blokiranje spoljnih poruka.
  
Kada kreirate pravilo u Exchange online centru administracije, slijedite ove korake da biste konfigurisali ETR da se primenjuje u usluzi Yammer:
  
- Prijavite se na Yammer kao verifikovan administrator i u **Yammer centru administracije** **Izaberite stavku \> Postavke sadržaja C i bezbednosti.**

- U okviru **spoljna razmena poruka**, izaberite **primenu primene Exchange online Exchange pravila transporta (etrs) u usluzi Yammer.**

- Odaberite stavku **Sačuvaj**.

Više informacija potražite u članku [Onemogućavanje spoljnih poruka u Yammer mreži](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  