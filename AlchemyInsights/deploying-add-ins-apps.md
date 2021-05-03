---
title: Primena programski dodatak za Microsoft 365 aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125684"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Primena programski dodatak za Microsoft 365 aplikacije

Centralizovana primena je preporučeni način za primenu Kancelarija za korisnike i grupe u organizaciji. Da biste primenili programski dodatak, pratite sledeće korake:

**Napomogućeno:** Da biste instalirali programske Kancelarija kao pojedinačni korisnik, pogledajte prikaz programskih dodatak, upravljanje i instaliranje programskih dodatak u [Kancelarija programima.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Takođe se uverite da je omogućena pojedinačna Kancelarija prodavnice programski dodaci. 

1. Uverite se da okruženje ispunjava zahteve za primenu programski dodatka pomoću centralizovane primene. Za detalje pogledajte [Zahtevi.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Idite na **Postavke** integrisane aplikacije Nabavite aplikacije u Microsoft 365 centra za  >    >   administaciju da biste primenili programski dodatak. 

Napomene: 

- Integrisane aplikacije zahtevaju da korisnik ima dozvole globalnog Exchange ili da Exchange za adminitre.

- Prilikom primene programskih dodatak za više korisnika, preporučujemo da dodele donose pomoću grupa umesto pojedinačnih korisnika. Za detalje pogledajte [razmatranja prilikom dodele programskih dodatka korisnicima i grupama.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Centralizovana primena ne podržava korisnike u ugnežđenim grupama ili grupama koje imaju nadređene grupe. Za detalje pogledajte [dodele za korisnika i grupu.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Uverite se da je Microsoft 365 Usluga za upravljanje aplikacijama (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') omogućena korisnicima da se prijave. Za detalje pogledajte Konfigurisanje [svojstava aplikacije.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Ako naižete na probleme sa primenu programski dodatka pomoću integrisanih aplikacija, pokušajte da primenite [koristeći programski dodatak.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Za više informacija pogledajte:

[Primena programskog dodatka u centru za administvene programe](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Upravljanje programski dodacima u centru aktivnosti](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Koristite PowerShell cmdlet cmdlet za centralizovanu primenu za upravljanje programski dodacima](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Objavljivanje Kancelarija korišćenjem centralizovane primene putem Microsoft 365 centra administracije](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Rešavanje problema: Korisnik ne vidi programski dodatak](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Rešavanje problema sa greškama korisnika Kancelarija programski dodaci](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)