---
title: Pretraga i brisanje e-poruka u organizaciji
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525440"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Pretraga i brisanje e-poruka u organizaciji

Sledite ove korake:

1. Ako niste globalni administrator, da biste pretražili poruke, nalog mora biti dodat u **grupu uloga programa Ediscovery Manager** ili **ulogu upravljanja usaglašenosti**. Da biste izbrisali poruke, moraćete da se pridružite **grupi uloga za upravljanje organizacijom** ili svojoj **ulozi za pretraživanje i čišćenje**. Dozvole za ove uloge se dodeljuju u [centru za bezbednost & bezbednosti.](https://protection.office.com)
2. [Kreirajte pretragu sadržaja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku za brisanje.
3. [Povezivanje sa bezbednosnim & PowerShell Center usaglašenosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Ako koristite MFA, pogledajte ova uputstva: [Povezivanje sa bezbednosnim & PowerShell Center za usaglašenost pomoću multifaktor potvrde identiteta](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Izbriši poruku: Pokreće `New-ComplianceSearchAction` cmdlet da biste izbrisali poruku. Izbrisane poruke se premeštaju u fasciklu "stavke koje se mogu spasti korisnik". Za primer komande pogledajte odeljak [3: brisanje poruke.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
