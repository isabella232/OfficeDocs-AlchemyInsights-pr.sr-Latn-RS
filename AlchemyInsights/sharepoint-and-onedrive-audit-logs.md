---
title: Klasiиni izveštaji o SharePoint nadzornoj evidenciji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662222"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint i OneDrive evidencija nadzora

## <a name="sharepoint-classic-audit-logs"></a>SharePoint Classic evidencija nadzora

Zastarelo nadgledanje SPO-a je migriralo u objedinjenu evidenciju nadzora (UAL). Svi izveštaji SPO-ve za zastareli nadzor će se sada primeniti na UAL, a signali zastarelog nadzora su migrirali u UAL.

Promene ključnih stavki:

* Skraćivanje skraćivanja nije dostupno kao mogućnost.
* Biranje određenih događaja za nadgledanje nije dostupno. Pogledajte [ovaj dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) za kompletnu listu revizija događaja dostupnih po podrazumevanoj vrednosti.
* Opcija **lokacije** u okviru **prilagođeni izveštaji** nije dostupna.
* Opcija " **Otvaranje" ili "preuzimanje dokumenata** " nije dostupna.

[Konfigurisanje postavki nadgledanja za kolekciju lokacija](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint i OneDrive moderne evidentirate nadzora iz usaglašenosti

* [Uključivanje/isključivanje objedinjenog evidentiranja nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

U sistemu SharePoint ili OneDrive nije potrebna dodatna konfiguracija.

Korišćenje pretrage evidentiranja nadzora radi provere aktivnosti datoteka, fascikli, korisnika, dozvola:

* [Aktivnosti datoteka i stranica](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Aktivnosti fascikle](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktivnosti deljenja i pristupa](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivnosti sinhronizacije](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktivnosti administracije sajta](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Više informacija o tome kako da preuzmete ove događaje potražite [u članku Pretraga evidencije nadzora](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
