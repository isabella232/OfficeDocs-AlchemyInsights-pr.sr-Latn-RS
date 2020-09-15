---
title: Ističe ADFS certifikat saveza
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686763"
---
# <a name="adfs-federation-certificate-expiring"></a>Ističe ADFS certifikat saveza

Da biste rešili ovaj problem, slijedite ove korake:
  
1. Instalirajte Microsoft Azure Active Directory modul za Windows PowerShell na računaru (ako modul nije već instaliran). Da biste to uradili, izaberite stavke [Azure AD pomoću programa Windows PowerShell](https://aka.ms/aadposh).

2. Pratite korake u odeljku "scenario 1: da certifikat za potpisivanje oglasa i potpisa istekne istekao" ["Došlo je do problema prilikom pristupanja lokaciji" iz oglasa "AD FS kada se savezni korisnik prijavljuje u Microsoft 365, Azure ili Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Pratite korake u programu [Ažuriraj ili popravite postavke savezenog domena u programu Microsoft, Azure ili Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Da biste saznali više o obnavljanju certifikata Federacije, pogledajte članak [obnavljanje certifikata Federacije za Microsoft 365 i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
