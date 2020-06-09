---
title: Primena timova kao samostalnih ili sa novim ili postojećim Office instalacijama
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617909"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Primena timova kao samostalnih ili sa novim ili postojećim Office instalacijama

Microsoft timovi sada su uključeni u ***nove instalacije*** Microsoft 365 aplikacija za Enterprise, Microsoft 365 aplikacije za preduzeća i Office za Mac. Više informacija potražite u članku [kada će Microsoft timovi početi da budu uključeni u nove instalacije sistema Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Pored toga, počev od verzije 1906 u trenutnom kanalu, timovi će biti ***dodati postojećim instalacijama*** Microsoft 365 aplikacija za Enterprise (i Microsoft 365 aplikacije za posao) na uređajima koji rade pod operativnim sistemom Windows kada ažurirate postojeću instalaciju na najnoviju verziju. Za više informacija pogledajte odeljak [Šta je sa postojećim instalacijama sistema Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ako ne želite da sačekate ovaj raspored, možete da primenite timove kao samostalni za korisnike tako što ćete [slediti ova uputstva](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ili možete imati svoje korisnike da sami instaliraju timove za sebe  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ako vaša organizacija nije spremna da rasporedi timove, imamo korake koje možete da preduzmete da biste ***izuzeli timove*** iz [novih](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ili [postojećih](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacija sistema Office. Ako želite da se timovi instaliraju, ali ne želite da se timovi automatski pokreću za korisnika nakon instalacije, pogledajte odeljak [Sprečavanje automatskog pokretanja Microsoft timova nakon instalacije](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Da biste ***deinstalirali timove*** sa uređaja koji radi pod operativnim sistemom Windows, pogledajte odeljak [Deinstaliranje Microsoft timova](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Da biste čistili Microsoft timove sa više ciljanih mašina ili korisnika, pogledajte [Čišćenje Microsoft timova za raspoređivanje](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ako koristite deljene računare, usluge udaljene radne površine (RDS) ili virtualnu infrastrukturu radne površine (VDI), pogledajte [deljene računarske i Vdi okruženja sa Microsoft timovima](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ako koristite Office za Mac računar, pogledajte [instalacije Microsoft timova na Mac računaru](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Nakon instalacije timova, [automatski se ažurira](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približno svake dve nedelje novim karakteristikama i kvalitetom kvaliteta. 