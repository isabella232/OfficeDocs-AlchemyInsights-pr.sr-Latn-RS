---
title: Primena timova kao samostalne ili sa novim ili postojećim Office instalacijama
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806773"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Primena timova kao samostalne ili sa novim ili postojećim Office instalacijama

Microsoft timovi su sada ***uključeni u radnju*** Microsoft 365 aplikacija za Enterprise, Microsoft 365 aplikacije za preduzeća i Office za Mac. Više informacija potražite u članku [kada će Microsoft timovi početi sa novim instalacijama sistema Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Pored toga, počev od verzije 1906 u trenutnom kanalu, timovi će biti ***dodati u postojeće instalacije*** Microsoft 365 aplikacija za Enterprise (i Microsoft 365 aplikacije za preduzeća) na uređajima koji rade pod operativnim sistemom Windows kada ažurirate postojeću verziju. Više informacija potražite u članku [koje su postojeće instalacije sistema Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ako ne želite da čekate ovaj plan za pomeranje, možete da primenite timove kao samostalni za korisnike tako što ćete [slediti ova uputstva](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   ili možete da omogućite korisnicima da instaliraju timove za sebe  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ako vaša organizacija nije spremna za raspoređivanje timova, imamo korake koje možete preduzeti da biste ***isključili timove*** iz [novih](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) ili [postojećih](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) instalacija sistema Office. Ako želite da se timovi instaliraju, ali ne žele da se timovi automatski počinju prilikom instaliranja, pogledajte članak [Sprečavanje Microsoft timova da se automatski pokreće posle instalacije](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

Da biste ***deinstalirali timove*** sa uređaja koji ima Windows, pogledajte članak [Deinstaliranje Microsoft timova](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Da biste očistili Microsoft timove od više ciljnih mašina ili korisnika, pogledajte članak [raspoređivanje Microsoft tima](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ako koristite deljene računare, usluge udaljene radne površine (RDS) ili virtuelnu infrastrukturu za računare (VASDI), pogledajte [deljene računare i vanske okruženije pomoću Microsoft timova](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ako koristite Office za Mac, pogledajte [Microsoft instalacije na Mac računaru](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Kada se timovi instaliraju, automatski se [ažurira](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) približno svake dve sedmice novim ispravkama za funkcije i kvalitet. 