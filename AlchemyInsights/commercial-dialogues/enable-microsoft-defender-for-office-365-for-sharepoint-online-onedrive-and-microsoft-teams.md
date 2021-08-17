---
title: Omogućite Microsoft zaštitnik za Office 365 za SharePoint Mreži, OneDrive i Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058880"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućite Microsoft zaštitnik za Office 365 za SharePoint Mreži, OneDrive i Microsoft Teams

1. Prijavite se u Office 365 centar za bezbednost i usaglašenost pomoću akreditiva globalnog ili [bezbednosnog administatora.](https://protection.office.com/)
2. Izaberite **stavku Upravljanje pretnjama** u levom oknu, a zatim **izaberite stavku**  >  [Smernice Sef priloge.](https://protection.office.com/safeattachment)
3. Izaberite **stavku Uključi Microsoft zaštitnik za Office 365 za SharePoint, OneDrive i Microsoft Teams ,** a zatim izaberite stavku **Sačuvaj**.
    > [!TIP]
    >
    > - Kao globalni ili SharePoint na mreži, pokrenite sledeći PowerShell cmdlet sa **DisallowInfectedFileDownload** parametar postavljenim na *vrednost true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Podešavanje obaveštenja za otkrivene datoteke](https://go.microsoft.com/fwlink/?linkid=2092110)

Dodatne informacije potražite u [članku Microsoft Office 365 za SharePoint, OneDrive i Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
