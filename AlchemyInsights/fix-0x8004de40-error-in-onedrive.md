---
title: Otklonite 0x8004de40 greške u usluzi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649762"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Otklonite 0x8004de40 greške u usluzi OneDrive

Ako imate Windows 7 i dobijate ovu grešku, ažurirajte je da biste omogućili [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao podrazumevane bezbedne protokole u operativnom sistemu WinHTTP u operativnom sistemu Windows.

Ako imate Windows 10 i dobijate 0x8004de40 sa OneDrive:

- Ponovo poništite računar na koji to utiče dok ste povezani sa Acitve Directory domenom.
- Ako poništavanje ne reši problem, ponovo se pridružite uređaju iz usluge Azure AD i ponovo se pridružite uređaju. 

**Napomi:** Trebalo bi da budete na mreži preduzeća dok izvršavate ove korake. Nemojte da izvršite ove korake kada niste povezani sa infrastrukturom preduzeća (na primer, prilikom putovanja). 

1. Otvorite komandnu liniju sa punim privilegijama tako što ćete izabrati start **,** kliknite desnim tasterom miša na stavku **Komandna** linija , a zatim izaberite **stavku Pokreni kao administrator**.

1. Otkucajte *dsregcmd /leave* i pritisnite **taster Enter**.

1. Kada završite, *otkucajte dsregcmd /join i* pritisnite **taster Enter.**

1. Kada se dovrše, zatvorite komandnu liniju.

1. Ponovo poništite računar i prijavite se u OneDrive.