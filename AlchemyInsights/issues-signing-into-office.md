---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744660"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemi sa prijavljivanjem u Microsoft 365 aplikacije

Na primer: Ako koristite stariju verziju programa Windows (na primer Windows 7 SP1, Windows Server 2008 R2), koristite jednostavnu popravku da biste kao podrazumevano omogućili TLS 1.2. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Više informacija potražite u temi Ažuriranje da biste omogućili [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao podrazumevane bezbedne protokole u winHTTP-u Windows.

Da biste rešili probleme sa prijavljivanjem Microsoft 365 aplikacije, isprobajte sledeće opcije na računaru na koji ovo utiče:  

- Dodatne Windows pogledajte u Preporuke o rešavanju uobičajenih problema [sa prijavljivanjem](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Za Mac, pogledajte [tj. Ne mogu da se prijavim u aplikaciju Kancelarija 2016 za Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Savet** Na računarima sa operativnim sistemom Windows, možemo da dijagnostikujemo nekoliko uobičajenih problema sa prijavljivanjem u Office i da ih automatski otklonimo za vas. Preuzmite i pokrenite aplikaciju  **[Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA-OfficeSignInScenario)** da biste koristili našu automatizovanu alatku.

**Napomogućeno:** Ne preporučuje se zabrana moderne potvrde identiteta (ADAL) ili upravljanja veb nalozima (WAM) za rešavanje problema sa prijavljivanjem ili **aktivacijama.** Ako se greške pojave prilikom povezivanja sa Microsoft 365 korišćenjem Kancelarija 2013, proverite da li ste omogućili [modernu](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) potvrdu identiteta Kancelarija klijentu.

Za određene radnje rešavanja problema pogledajte:

[Problemi sa povezivanjem pri prijavljivanjem nakon ažuriranja na Kancelarija 2016 izdanje 16.0.7967 u programu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Ne možete da se prijavite na nalog organizacije kao što Office 365, Azure ili Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Rešavanje problema sa aplikacijama koje nisu pregledači koje ne mogu da se prijade u Office 365, Azure ili Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Više puta su zatraženi akreditivi u Kancelarija](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)