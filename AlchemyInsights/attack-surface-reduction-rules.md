---
title: Pravila za smanjenje površine napada
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676441"
---
# <a name="attack-surface-reduction-rules"></a>Pravila za smanjenje površine napada

Isključivanje datoteka ili fascikli može ozbiljno da smanji zaštitu koju pružaju pravila za smanjenje površine napada. Datotekama koje je pravilo blokiralo dozvoljeno je da se pokrenu i nijedan izveštaj ili događaj se ne zapisuje. Izuzetke se primenjuju na sva pravila koja dozvoljavaju izuzetke.

ASR izuvici koriste istu sintaksu kao Antivirusni program Microsoft zaštitnika izusci. Za detalje pogledajte Konfigurisanje i provera valjanosti izuzetka [za Antivirusni program Microsoft zaštitnika skeniranja.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Da biste izbegli probleme, [pregledajte uobičajene greške koje treba da izbegnete pri definisanju izuzetaka.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Ne podržavaju sva ASR pravila izuzetke. Da biste proverili da li pravilo podržava izuzetke, pogledajte tabelu Pravila za smanjenje površine [napada.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Pravila za smanjenje površine napada

Površina napada u organizaciji obuhvata sva mesta na kojima napadač može da ugrozi organizacione uređaje ili mreže. Smanjivanje površine napada znači zaštita uređaja i mreže organizacije, što ostavlja napadače sa manje načina za vođenje napada. Konfigurisanje pravila za smanjenje površine napada u Programu Microsoft zaštitnik za krajnju tačku može pomoći.

Za više informacija pogledajte:

- [Mapiranje GUID-a ASR pravila za ime](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Zahtevi za ASR pravila:
    - [Windows 10 Pro, verzija 1709 ili novija](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, verzija 1709 ili novija](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, verzija 1803 (polugodišnji kanal) ili novija](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Identifikovanje odgovarajućeg izuzetka za primenu

1. Potražite ID događaja 1121 ili 1122 u Microsoft-Windows-Windows zaštitnik/Operational evidenciji.

1. Procenite scenario blokiranja i kontekst i potvrdite da ovaj scenario treba da se deblokira.

1. Pročitajte vrednost Putanja u detaljima događaja, što je vrednost koja definiše izuzetak.
    - Učinite izuzetke što je moguće strogim.
    - Primenite džoker znak tamo gde je potrebno (na primer, zamenite promenljivu Korisnik).

1. Primenite izuzetak u skladu sa potrebama za primenom. Za detalje pogledajte Prilagođavanje [pravila za smanjenje površine napada.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Izuvišnost se ne poštuje

1. Utvrdite da li pravila podržavaju izuzetke. Za detalje pogledajte pravila [za smanjenje površine napada.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Pregledajte primenjene izuzetke i verifikujte sa podacima o događaju da biste unosili pogrešno protumačene džoker znakove. Više informacija potražite u [članku Podržani tipovi izuzetka](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. ako je uticaj pravila previsoko, razmotrite premeštanje pravila (nazad) u režim nadzora radi dalje provere valjanosti. Detalje možete da vidite u [članku Testiranje načina na koji funkcije Microsoft zaštitka za krajnje tačke rade u režimu nadzora.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Prikupite podatke podrške da biste otvorili predmet podrške pomoću ove komande:
    
   ** MDEClientAnalyzer.cmd -v**

    Više informacija potražite u [članku Problemi sa mašinama za ulaženje u Microsoft zaštitnik za krajnje tačke.](issues-with-onboarding-machines.md)
