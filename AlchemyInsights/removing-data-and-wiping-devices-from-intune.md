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
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922265"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Uklanjanje podataka i brisanje uređaja iz usluge Intune

Udaljene radnje „Uklanjanje uređaja“ i „Brisanje uređaja“ mogu se koristiti za uklanjanje podataka preduzeća kojima upravlja Intune ili za vraćanje na fabrička podešavanja i vraćanje uređaja na podrazumevane postavke.

1. Prijavite se u Microsoft 365 upravljanje uređajima i idite na **Uređaji** > **Svi uređaji**.
2. Izaberite uređaj koji želite da izbrišete.
3. Izaberite tip daljinskog brisanja koje želite da izvršite. Poništavanje briše samo organizacione informacije, dok se potpunim brisanjem uređaj vraća na fabrička podešavanja.
4. Kliknite na dugme **Da** kako biste potvrdili. Dok se brisanje ne završi, status radnje uređaja prikazuje se kao *Povlačenje na čekanju*.
    Kada se radnja dovrši, više nećete videti mobilni uređaj na listi upravljanih uređaja.

> [!NOTE]
> Podaci preduzeća ne mogu se ukloniti sa uređaja PRIDRUŽENIH za Azure AD. 

Za sve detalje o efektu radnji povlačenja i brisanja, uključujući ono što se zadržava i šta se briše, pogledajte sledeću dokumentaciju:

- [Uklonite uređaje brisanjem, povlačenjem ili ručnim odjavljivanjem uređaja.](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Kako obrisati samo korporativne podatke iz aplikacija kojima upravlja Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Izbrišite sve podatke sa macOS uređaja](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).