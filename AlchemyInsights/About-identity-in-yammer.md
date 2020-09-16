---
title: O identitetu u usluzi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664184"
---
# <a name="about-identity-in-yammer"></a>O identitetu u usluzi Yammer

Preporučuje se da sve mreže preduzmu sledeće korake da bi se izbegli problemi u vezi sa identitetom:

1. Nametanje Office 365 identiteta nakon obezbeđivanja Microsoft 365 naloga za korisnike u Azure AD da biste se uverili da se svi korisnici prijave pomoću primarnog Microsoft 365 naloga. Više informacija potražite u članku [nametanje primene Office 365 identiteta za Yammer korisnike](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidovanje više Yammer mreža. Zastarele konfiguracije usluge Yammer dozvoljava da se više Yammer mreža poveže sa jednim zakupcem. Više informacija potražite u članku [migracija na mreži – konsolidacija više Yammer mreža](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opcionalno, nametanje licenciranja za Yammer da blokirate korisnike iz usluge Yammer ako nemaju licencu. Više informacija potražite u članku [Upravljanje korisničkim licencama usluge Yammer u sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Konačno, nadzor liste korisnika za starije Yammer mreže i suspenduje zastarele korisnike. Preporučuje se da obustavite (Deaktivirajte) korisnike umesto da ih brišete zato što je brisanje neopoziva. Više informacija potražite u članku [nadgledanje Yammer korisnika u mrežama povezanim sa sistemom Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [uklanjanjem korisnika](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfigurisanjem Yammer pomoću ovih koraka takođe ćete biti spremni da konfigurišete Yammer mrežu za izvorni režim za Microsoft 365. Više informacija potražite u članku [Konfigurisanje Yammer mreže za izvorni režim za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).