---
title: Omogućavanje korisniku da sinhronizuje lični nalog sa poslovnim nalogom u programu Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813405"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Omogućavanje korisniku da sinhronizuje lični nalog sa poslovnim nalogom u programu Microsoft Edge

Uverite se da ispunjavate ove kriterijume:

- Enterprise State Roaming je omogućen u Azure Active Directory centru za adminitre, što zahteva pretplatu na Azure Active Directory Premium ili Enterprise Mobility + Security (EMS). Više informacija potražite u članku [Omogućavanje usluge Enterprise State Roaming u Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Ispunjeni su neki od sledećih kriterijuma:
    - Azure Information Protection usluga je omogućena za vašeg zakupca. Za detalje pogledajte [aktiviranje zaštite Azure Rights Management iz Microsoft 365 centar administracije.](/azure/information-protection/activate-office365)
    - Funkcija Azure Active Directory Enterprise State Roaming (ESR) omogućena je za svakog korisnika ili zakupca. Dodatne informacije potražite u [članku Šta je to stanje preduzeća u romingu?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Ako su onemogućene AIP i ESR, poruka o grešci obaveštava korisnike da sinhronizacija nije dostupna za njihove naloge.
