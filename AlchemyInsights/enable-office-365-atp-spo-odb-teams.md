---
title: Omogućite Office 365 ATP za SharePoint, OneDrive i Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332173"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućite Microsoft zaštitnik za Office 365 za SharePoint Online, OneDrive i Microsoft Teams

1. Idite na https://protection.office.com i prijavite se.
2. Odaberite **stavku**  >  **Smernice za upravljanje**  >  **pretnjama Sef prilozima.**
3. Izaberite **stavku Uključi zaštitnik za Office 365 za SharePoint, OneDrive i Microsoft Teams**, a zatim kliknite na dugme **Sačuvaj.**
4. (Preporučeno) Kao globalni administrator ili administrator SharePoint na mreži, pokrenite cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) sa **disallowInfectedFileDownload** parametar postavljenim na *vrednost true.*
5. (Preporučeno) [Podesite obaveštenja za](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) otkrivene datoteke.

**Nabrajanje:** Microsoft zaštitnik za Office 365 neće skenirati svaku datoteku u uslugama SharePoint Online, OneDrive ili Microsoft Teams. Datoteke se skeniraju as sinhrono, kroz proces koji koristi događaje deljenja i aktivnosti gosta, zajedno sa pametnom heuristicom i signalima pretnji za identifikovanje zlonamernih datoteka. Pogledajte [članak Microsoft zaštitnik Office 365 za SharePoint, OneDrive i Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
