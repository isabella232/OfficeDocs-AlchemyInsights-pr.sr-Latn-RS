---
title: Ispravka greške 0x8004de40 u usluzi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745144"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Ispravka greške 0x8004de40 u usluzi OneDrive

Ako primite grešku 0x8004de40 0 uz OneDrive:

- Ponovo pokrenite računar koji utiče na njega dok ste povezani sa Acitve Domain Domain Directory.
- Ako ponovno pokretanje ne reši problem, odpridružite se i pridružite se uređaju iz usluge Azure AD. 

**Napomena**: trebalo bi da budete na mreži preduzeća prilikom izvršavanja ovih koraka. Nemojte vršiti ove korake kada ne možete da se povežete sa korporativnom infrastrukturom (na primer, dok putujete). 

- Otvorite otvorenu komandnu liniju. 
- Da biste otvorili povećanu komandnu liniju, kliknite- **Start**, kliknite desnim tasterom miša na **komandnu liniju**, a zatim izaberite stavku **Pokreni kao administrator**.
- Otkucajte *dsregcmd/ostavi* i pritisnite taster **ENTER**.
- Kada završite, otkucajte *dsregcmd/JOIN* i pritisnite taster **ENTER**.
- Kada završite, zatvorite komandnu liniju.
- Ponovo pokrenite računar i prijavite se u OneDrive.