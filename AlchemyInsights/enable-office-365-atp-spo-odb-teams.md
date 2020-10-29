---
title: Omogućavanje sistema Office 365 ATP za SharePoint, OneDrive i Microsoft timove
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801071"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućavanje Microsoft zaštitnika za Office 365 za SharePoint online, OneDrive i Microsoft timove

1. Idite na https://protection.office.com i prijavite se.
2. Odaberite stavku smernice **za upravljanje pretnjama** i  >  **Policy**  >  **bezbednost** .
3. Izaberite stavku **UKLJUČI ATP za SharePoint, OneDrive i Microsoft timove** , a zatim kliknite na dugme **Sačuvaj** .
4. Preporučuje Kao globalni administrator ili SharePoint online administrator, uradite " [setu-Spojstanar](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) " cmdlet pomoću parametra za **Disallowinittedpreuzeto** na *TRUE* .
5. Preporučuje [Podesite upozorenja](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkrivene datoteke.

> [!NOTE]
> ATP će nZa skeniranje svake datoteke u usluzi SharePoint online, OneDrive ili Microsoft tima. Datoteke su isiskirale asihrono, kroz proces koji koristi deljenje i događaje sa gostima, zajedno sa pametnim houristikom i signalima pretnje za identifikovanje zlonamernih datoteka. Pogledajte [ATP za SharePoint, OneDrive i Microsoft timove](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).