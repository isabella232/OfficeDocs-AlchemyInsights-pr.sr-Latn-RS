---
title: Slanje prilagođenih obaveštenja u intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086178"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Kako slati prilagođena obaveštenja korisnicima kontrolisanih iOS i Android uređaja

Prilagođena obaveštenja za Intune obrađuje aplikacija Company Portal na uređaju korisnika. Aplikacija zatim kreira push obaveštenje na tom uređaju.

Ovo su preduslovi uređaja za podršku potvrde prilagođenih obaveštenja i da aplikacija zatim kreira push obaveštenje:

- Uređaj mora da ima instaliranu Company Portal aplikacije.  

- Uređaj mora da dozvoli aplikaciji Company Portal slanje push obaveštenja. Kada se aplikacija instalira ili ažurira, od korisnika će zatražiti da dozvoli obaveštenja.

- Android uređaji moraju da imaju instalirane Google Play usluge.

- Uređaj mora da bude upisan za Intune.

Dodatne informacije, uključujući i način slanja poruke, potražite u [dokumentaciji za funkcije.](https://docs.microsoft.com/intune/custom-notifications)
