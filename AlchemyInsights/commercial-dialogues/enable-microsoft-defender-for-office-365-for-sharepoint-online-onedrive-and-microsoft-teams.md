---
title: Omogućavanje Sef prilozima za SharePoint Online, OneDrive i Microsoft Teams
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332393"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućavanje Sef prilozima za SharePoint Online, OneDrive i Microsoft Teams

1. Korišćenjem akreditiva globalnog ili bezbednosnog administatora, otvorite Microsoft 365 zaštitnik portal na , a zatim idite na odeljak Smernice za smernice & smernice za pretnje <https://security.microsoft.com>  \>  \> **Sef**  Prilozi u odeljku Smernice

   Da biste prešli direktno **na stranicu Sef Prilozi,** koristite <https://security.microsoft.com/safeattachmentv2> .

2. Na stranici **Sef Prilozi** izaberite stavku **Globalne postavke.**
3. U iletu koji se pojavi izaberite stavku Uključi Microsoft zaštitnik za Office 365 za **SharePoint, OneDrive i Microsoft Teams ,** a zatim izaberite stavku **Sačuvaj**.

    **Savet:** Uradite sledeće da biste poboljšali zaštitu zaštite Sef za SharePoint, OneDrive i Microsoft Teams:
    - Da biste sprečili korisnike da preuzmu zlonamerne datoteke, koristite vrednost za `$true` *DisallowInfectedFileDownload* parametar na cmdlet komandi **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** u programu SharePoint Online PowerShell. Više informacija potražite u temi Korišćenje programa SharePoint PowerShell za sprečavanje korisnika da [preuzmu zlonamerne datoteke.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [Kreiranje smernica upozorenja za otkrivene datoteke](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Više informacija potražite u Sef Prilozi za [Office 365 za SharePoint, OneDrive i Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
