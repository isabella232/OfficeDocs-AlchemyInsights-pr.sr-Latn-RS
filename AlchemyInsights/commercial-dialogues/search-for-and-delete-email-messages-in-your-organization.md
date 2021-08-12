---
title: Traženje i brisanje e-poruka u organizaciji
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
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948897"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Traženje i brisanje e-poruka u organizaciji

Sledite ove korake:

1. Ako niste globalni dobavljač, da biste pretražili poruke koje imate na nalogu, morate da dodate u grupu uloga menadžera **e-pošte** ili ulogu upravljanja pretragom usaglašenosti.  Da biste izbrisali poruke, morate da se pridružite grupi uloga "Upravljanje **organizacijom"** ili ulozi upravljanja pretragom **i brisanjem.** Dozvole za ove uloge dodeljene su u centru & [za usaglašenost bezbednosti.](https://protection.office.com)
2. [Kreirajte pretragu sadržaja](https://docs.microsoft.com/office365/securitycompliance/content-search) da biste pronašli poruku za brisanje.
3. [Povezivanje u PowerShell & za usaglašenost.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Ako koristite MFA, pogledajte ova uputstva: Povezivanje centar za & usaglašenost programa [PowerShell pomoću višestruke potvrde identiteta](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Izbrišite poruku: pokrenite `New-ComplianceSearchAction` cmdlet da biste izbrisali poruku. Izbrisane poruke se premeštaju u fasciklu "Stavke koje mogu da se oporave" korisnika. Za primer komande, pogledajte [3. korak: Brisanje poruke.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
