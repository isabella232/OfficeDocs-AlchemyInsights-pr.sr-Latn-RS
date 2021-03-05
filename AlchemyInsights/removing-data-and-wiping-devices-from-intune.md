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
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416327"
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