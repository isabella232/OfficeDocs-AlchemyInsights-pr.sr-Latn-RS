---
title: Uklanjanje podataka i brisanje uređaja iz usluge Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331055"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Uklanjanje podataka i brisanje uređaja iz usluge Intune

Udaljene radnje „Uklanjanje uređaja“ i „Brisanje uređaja“ mogu se koristiti za uklanjanje podataka preduzeća kojima upravlja Intune ili za vraćanje na fabrička podešavanja i vraćanje uređaja na podrazumevane postavke.

1. Prijavite se u Microsoft 365 upravljanje uređajima i idite na **Uređaji** > **Svi uređaji**.
2. Izaberite uređaj koji želite da izbrišete.
3. Izaberite tip daljinskog brisanja koje želite da izvršite. Poništavanje briše samo organizacione informacije, dok se potpunim brisanjem uređaj vraća na fabrička podešavanja.
4. Kliknite na dugme **Da** kako biste potvrdili. Dok se brisanje ne završi, status radnje uređaja prikazuje se kao *Povlačenje na čekanju*.
    Kada se radnja dovrši, više nećete videti mobilni uređaj na listi upravljanih uređaja.

**Napom:** Podaci preduzeća ne mogu da se uklone sa uređaja PRIDRUŽENIH U Azure AD. 

Za sve detalje o efektu radnji povlačenja i brisanja, uključujući ono što se zadržava i šta se briše, pogledajte sledeću dokumentaciju:

- [Uklonite uređaje brisanjem, povlačenjem ili ručnim odjavljivanjem uređaja.](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Kako obrisati samo korporativne podatke iz aplikacija kojima upravlja Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Izbrišite sve podatke sa macOS uređaja](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).