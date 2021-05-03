---
title: Problemi sa SharePoint na Windows 7 uređajima
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125516"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problemi sa SharePoint na Windows 7 uređajima

Ako dobijete greške na Windows 7 računara dok radite na SharePoint ili OneDrive, one su možda povezane sa ukidanje TLS 1.0/1.1. Za više informacija pogledajte:

- [Priprema za TLS 1.2 u Office 365 i Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 klijentima moraju biti omogućeni TLS1.2. Dodatne informacije potražite u temi Greške potvrde identiteta kada klijent [nema podršku za TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Instalirajte KB3140245 i kreirajte vrednost registratora. Više informacija potražite u temi Ažuriranje da biste omogućili [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) kao podrazumevane bezbedne protokole u winHTTP-u Windows

- Windows 7 SP1/Windows 8 klijenti moraju da obezbede da su instalirani najnoviji TLS cipher paketi. Dodatne informacije potražite u članku Microsoft savet za [bezbednost 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


