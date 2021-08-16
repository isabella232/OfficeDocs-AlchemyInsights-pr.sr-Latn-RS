---
title: Primena Teams kao Kancelarija ili sa novim ili postojećim Kancelarija instalacijama
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
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102216"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Primena Teams kao Kancelarija ili sa novim ili postojećim Kancelarija instalacijama

Microsoft Teams je sada uključen u nove  instalacije sistema Microsoft 365 Apps za preduzeće, Microsoft 365 aplikacije za posao i programa Kancelarija za Mac. Više informacija potražite u [temi Kada Microsoft Teams počne da se uključuje uz nove instalacije programa Kancelarija?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Pored toga, Teams će, počevši od verzije 1906 u trenutnom kanalu, biti dodat u postojeće instalacije sistema Microsoft 365 Apps za preduzeće (i Microsoft 365 aplikacije za posao) na uređajima koji rade Windows kada ažurirate postojeću instalaciju na najnoviju verziju.  Dodatne informacije potražite u [temi Šta se sa postojećim instalacijama Kancelarija?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ako ne želite da čekate ovaj raspored primene, možete da primenite Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) kao sami za korisnike tako što ćete pratiti ova uputstva ili možete da omogućite korisnicima da instaliraju Teams za [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) sebe.

Ako vaša organizacija nije spremna da primeni Teams, imamo ***korake*** koje možete da [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) preduzete [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) kako biste izuzeli Teams iz novih ili postojećih instalacija sistema Kancelarija. Ako želite da Teams instalirate, ali ne želite Teams da se pokrene automatski za korisnika nakon [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)instalacije, pogledajte sprečavanje Microsoft Teams automatskog pokretanja nakon instalacije.

Da ***biste Teams na*** uređaju koji radi Windows, pogledajte tj. Microsoft Teams. [](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) Da biste očistili Microsoft Teams više ciljnih računara ili korisnika, pogledajte Microsoft Teams [čišćenje primene.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Ako koristite deljene računare, usluge udaljene radne površine (RDS) ili Infrastruktura virtuelne radne površine (VDI), pogledajte tp Deljeni računar i [VDI](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)okruženja pomoću Microsoft Teams.

Ako koristite program Kancelarija Mac, pogledajte Microsoft Teams [instalacije na Mac računaru.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

> [!NOTE]
> Kada Teams instalira, on se automatski [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) ažurira otprilike svake dve nedelje novim funkcijama i ispravkama kvaliteta. 