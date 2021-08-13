---
title: O identitetu u Yammer
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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918951"
---
# <a name="about-identity-in-yammer"></a>O identitetu u Yammer

Preporučuje se da sve mreže preduzmu sledeće korake kako bi izbegle probleme u vezi sa identitetima:

1. Nameći Office 365 identitet nakon obezbeđivanja Microsoft 365 naloga za korisnike u Azure AD kako bi se obezbedilo da se svi korisnici prijave pomoću primarnog Microsoft 365 naloga. Više informacija potražite u [članku Primena Office 365 identiteta za Yammer korisnike.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Konsolidujte više Yammer mreža. Za Yammer konfiguracija dozvoljavaju da više Yammer bude povezano sa jednim zakučarom. Više informacija potražite u [članku Migracija mreže – Konsoliduj više Yammer mreža.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Opcionalno, naslonite Yammer da blokirate korisnike iz Yammer ako nemaju licencu. Više informacija potražite u članku [Upravljanje Yammer korisničkim licencama u Office 365.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)
4. Na kraju, nadgledate spisak korisnika za starije Yammer i obustavljate zatamnjene korisnike. Preporučuje se da obustavite (deaktivirate) korisnike umesto da ih brišete, jer brisanje nije moguće. Više informacija potražite u [člancima Nadzor Yammer korisnicima na mrežama povezanim sa uslugom Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [i Uklanjanje korisnika.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Ako konfigurišete Yammer ovim koracima, bićete spremni i da konfigurišete Yammer mrežu za utiv režim za Microsoft 365. Dodatne informacije potražite u [članku Konfigurisanje Yammer za urođivni režim za Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)