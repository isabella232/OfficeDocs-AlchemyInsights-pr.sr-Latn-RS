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
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892813"
---
# <a name="configure-endpoint-dlp"></a>Konfigurisanje DLP-a krajnje tačke

Microsoft DLP krajnje tačke vam omogućava da proširite DLP zaštitu i mogućnost nadgledanja na osetljive informacije na Windows 10 uređajima. Nakon što se uređaji postave u upravljanje uređajima, možete da kreirate smernice za DLP da biste na stavke nametnuli radnje zaštite. Istraživač aktivnosti može da se koristi za nadgledanje aktivnosti za osetljive stavke. Za više informacija, pogledajte [Postavljanje uređaja u upravljanje uređajima](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Da biste počeli da koristite DLP krajnje tačke:

- Uverite se da imate odgovarajuće licenciranje za SKU/pretplate. Za više informacija, pogledajte [Licenciranje za SKU/pretplate](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Proverite dozvole potrebne za omogućavanje upravljanja uređajem, pristup stranici za postavljanje ili nadgledanje uključivanja/isključivanja uređaja. Za više informacija, pogledajte [Dozvole](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Postavite uređaje u upravljanje uređajima prateći proceduru za postavljanje uređaja. Za više informacija, pogledajte [Postavljanje uređaja](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Kreirajte smernice za DLP da biste zaštitili osetljive stavke. Informacije potražite u članku [ Scenariji smernica za DLP krajnje tačke](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Za više informacija o Microsoft DLP-u krajnje tačke, pogledajte članak [Saznajte više o Microsoft 365 sprečavanju gubitka podataka krajnje tačke (pregled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Važni koraci za prikupljanje podataka, ako je potrebna podrška:**

1. Preuzmite [pregled MDATP klijenta Analyzer](https://aka.ms/betamdatpanalyzer).
1. Koristite alatku kao administrator iz cmd prozora:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Kada vam bude zatraženo **Unesite broj minuta** za prikupljanje praćenja: , unesite broj minuta potrebnih za pokretanje scenarija.
1. Pokrenite scenario.

Prikupite izlaz Zip datoteke da biste ga dali agentu za podršku.
