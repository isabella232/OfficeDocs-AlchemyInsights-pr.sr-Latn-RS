---
title: Funkcija DLP možda treba da bude prilagođen
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712198"
---
# <a name="dlp-might-need-a-custom-type"></a>Funkcija DLP možda treba da bude prilagođen

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Funkcija DLP može zahtevati prilagođeni tip informacija**

Pomoću smernica za sprečavanje gubitka podataka (DLP) možete da identifikujete i zaštitite osetljive podatke u organizaciji. U nekoliko slučajeva možda ćete morati da kreirate sopstveni **prilagođeni** tip informacija da biste zaštitili podatke organizacije.

Na primer, vaša organizacija će možda morati da identifikuje i zaštiti ID-ove zaposlenih ili druge podatke u nekom formatu koji je specifičan za org. Ako je tako, pogledajte sledeće članke za više informacija.
  
 **Prilagođavanje ugrađenog tipa informacija**
  
Ako tip ugrađene osetljive informacije odgovara vašim potrebama samo sa nekoliko dodataka, možete da [prilagodite ugrađeni tip informacija](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Na primer, možete da dodate ili uklonite ključne reči ili da dodate ili uklonite pomoćne dokaze kao što je datum ili adresa.
  
 **Kreiranje tipa prilagođene osetljive informacije**
  
Međutim, ako treba da identifikujete i zaštitite drugačiji tip osetljivih informacija, možete da [kreirate prilagođeni tip informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) u usluzi UI centra za usaglašenost &.
  
**Kreiranje prilagođene osetljive informacije u programu Security & centar za usaglašenost sa PowerShell**

Na kraju, ako UI ne obezbede sve opcije koje su vam potrebne, možete da [kreirate prilagođeni tip informacija u bezbednosnoj & PowerShell Center usaglašenosti](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Ako počnete sa XML datotekom, možete da koristite svaku dostupnu opciju.
