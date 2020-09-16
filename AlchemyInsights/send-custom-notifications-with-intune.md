---
title: Slanje prilagođenih obaveštenja Intune
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720660"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Kako da pošaljete prilagođena obaveštenja korisnicima kompletnih iOS i Android uređaja

Prilagođena obaveštenja za Intune obrađuje aplikacija portal preduzeća na uređaju korisnika. Aplikacija zatim kreira obaveštenje o pritiskom na tom uređaju.

Slede preduslovi za podršku prilikom prijema prilagođenih obaveštenja, a zatim za aplikaciju da biste zatim kreirali obaveštenje o pritisanju:

- Uređaj mora da ima instaliran aplikaciju za preduzeće portal.  

- Uređaj mora da omogući aplikaciji portala preduzeća da šalje push obaveštenja. Kada se aplikacija instalira ili ažurira, on će zatražiti od korisnika da dozvoli obaveštenja.

- Android uređaji mora da imaju instalirane Google Play usluge.

- Uređaj mora biti upisan u Intune.

Više informacija o tome kako da pošaljete poruku potražite u [dokumentaciji funkcije](https://docs.microsoft.com/intune/custom-notifications).
