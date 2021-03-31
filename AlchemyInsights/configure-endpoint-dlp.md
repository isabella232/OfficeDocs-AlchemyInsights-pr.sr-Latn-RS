---
title: Konfigurisanje DLP-a krajnje tačke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402451"
---
# <a name="configure-endpoint-dlp"></a>Konfigurisanje DLP-a krajnje tačke

Microsoft DLP krajnje tačke vam omogućava da proširite DLP zaštitu i mogućnost nadgledanja na osetljive informacije na Windows 10 uređajima. Nakon što se uređaji postave u upravljanje uređajima, možete da kreirate smernice za DLP da biste na stavke nametnuli radnje zaštite. Istraživač aktivnosti može da se koristi za nadgledanje aktivnosti za osetljive stavke. Za više informacija, pogledajte [Postavljanje uređaja u upravljanje uređajima](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Da biste počeli da koristite DLP krajnje tačke:

- Uverite se da imate odgovarajuće licenciranje za SKU/pretplate. Za više informacija, pogledajte [Licenciranje za SKU/pretplate](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Proverite dozvole potrebne za omogućavanje upravljanja uređajem, pristup stranici za postavljanje ili nadgledanje uključivanja/isključivanja uređaja. Za više informacija, pogledajte [Dozvole](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Postavite uređaje u upravljanje uređajima prateći proceduru za postavljanje uređaja. Ako vam nedostaje opcija (pregleda) postavljanja uređaja u okviru **Smernica** za M365 usaglašenost, potvrdite da imate odgovarajuću licencu i dozvole na koje se upućuje iznad. Za više informacija, pogledajte [Postavljanje uređaja](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Kreirajte smernice za DLP da biste zaštitili osetljive stavke. Informacije potražite u članku [ Scenariji smernica za DLP krajnje tačke](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Za više informacija o Microsoft DLP-u krajnje tačke, pogledajte članak [Saznajte više o Microsoft 365 sprečavanju gubitka podataka krajnje tačke (pregled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Važni koraci za prikupljanje podataka, ako je potrebna podrška:**

1. Preuzmite pregled analizatora MDATP klijenta sa [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Koristite alatku kao administrator iz cmd prozora:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Kada vam bude zatraženo „Unesite broj minuta da biste prikupili praćenja: “, unesite broj minuta koji je potreban za pokretanje scenarija
5. Pokretanje scenarija

Prikupite izlaz Zip datoteke koji treba predati agentu za podršku.
