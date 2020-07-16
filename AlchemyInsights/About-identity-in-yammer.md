---
title: O identitetu u mreži Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148304"
---
# <a name="about-identity-in-yammer"></a>O identitetu u mreži Yammer

Preporučuje se da sve mreže preduzmu sledeće korake da biste izbegli probleme vezane za identitet:

1. Nametni Office 365 identitet nakon što obezbedite Microsoft 365 naloge za korisnike u programu Azure oglasa da biste bili sigurni da se svi korisnici prijavljivanjem pomoću primarnog Microsoft 365 naloga. Više informacija potražite u članku [Primenjivanje Office 365 identiteta za korisnike mreže Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidovanje više mreža na mreži Yammer. Zastarele konfiguracije mreže Yammer dozvoljavaju da više mreža na mreži Yammer bude povezano sa jednim tenkom. Više informacija potražite u članku [migracija mreže-konsolidovanje više mreža Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Opcionalno, primenite licencu za Yammer da biste blokirali korisnike sa mreže Yammer ako nemaju licencu. Više informacija potražite u članku [Upravljanje korisničkim licencama za Yammer u sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Na kraju, revizite listu korisnika za starije mreže Yammer i obustavite zastarele korisnike. Preporučuje se da obustavite (deaktivirate) korisnike umesto da ih izbrišete, jer je brisanje neopoziva. Više informacija potražite u članku [nadgledanje korisnika Yammer na mrežama povezanim sa Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [Uklanjanje korisnika](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Ako konfigurišete Yammer pomoću ovih koraka, takođe ćete biti spremni da konfigurišete mrežu Yammer za osnovni režim za Microsoft 365. Više informacija potražite u članku [Konfigurisanje mreže Yammer za osnovni režim za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).