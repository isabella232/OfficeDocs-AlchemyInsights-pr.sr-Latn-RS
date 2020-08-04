---
title: Problemi pri korišćenju funkcije Intune admin Console
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555876"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemi pri korišćenju funkcije Intune admin Console

**"Pristup je odbijen" prilikom kretanja administratorskog portala Intune.**

- Ako ste član "Intune" prilagođene uloge, uverite se da je na nalog dodeljen licencu za Intune ili poslovnu mobilnost (EMS).
- Ako koristite upravljač za konfiguraciju za upravljanje uređajima, proverite da niste deo funkcije "Intune korisnika" za upravljač konfiguracije MDM.
- Proverite da li vam je dodeljena odgovarajuća dozvola za kontrolu administracije zasnovana na ulogama (RBAC) u oštricom za Intune.
- Provera grupe koja se koristi nije lista distribucije. Intune na Azure portalu podržava samo korisničke naloge koji pripadaju samo Azure bezbednosnim grupama aktivnog direktorijuma. Pregledajte grupe u > **Intune**  >  ili u**grupi**Azure portala > **Azure Active Directory**.

**Korisnik ima previše dozvola za dodeljenu ulogu Intune**

Posavetuje korisnika da ide u " **Intune**  >  **Intune" uloge**  >  **moje dozvole**  >  **Izvezi** da pregleda dodeljene dozvole.

**U ulogu je dodata grupa opsega, ali korisnici u toj ulozi i dalje vide druge korisnike ili uređaje.**

Grupe opsega ne filtriraju korisnike ili uređaje. Grupe opsega:

- Ograničite pristup kome korisnici mogu da dodeljuju smernice ili aplikacije.
- Dozvoli samo određenim korisnicima da pokrenu udaljene zadatke na uređajima.

Više informacija o grupama opsega potražite u članku [Kontrola pristupa zasnovana na ulozi (RBAC) sa programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Dodao sam korisnika u ulogu Intune, ali i dalje imaju potpuni pristup usluzi Intune admin Console.**

Dođite do Intune > **korisnika** na Azure portalu i proverite da li korisnik nije dodeljen ni jednom od sledećih uloga na Azure portalu:

- Globalni administratorski
- Administrator Intune usluge
- SharePoint administratoru

Više informacija potražite u članku [Kontrola pristupa zasnovana na ulogama (RBAC) sa programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problemi sa pristupom**

Više informacija potražite u članku [ne možete da se prijavite na Office 365, Azure ili Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).