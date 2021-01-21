---
title: Konfigurisanje i proširivanje simbola ћivotnih vekova
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917010"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfigurisanje i proširivanje simbola ћivotnih vekova

Možete da precizirate životni vek Access, SEMLA ili Token ID-a koji izdaje Microsoft platforma za identifikaciju. Možete da postavljate Token ћivotna za sve aplikacije u organizaciji, za aplikaciju za više stanara (multi-organizacija) ili za određenu uslugu usluge u organizaciji. Da biste dobili više informacija, pročitajte simbol za čitanje u [čitljivom](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)programu.

Primere pročitajte [Kako da konfigurišete Token ћivota](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Da biste saznali kako da konfigurišete trajanje i kompatibilnost simbola u članku Azure Active Directory B2C (Azure AD B2C), pogledajte članak [Konfigurisanje simbola u usluzi Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Članak [konfiguriše ponašanje sesije u usluzi Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) opisuje metode za jedinstveno prijavljivanje (SSO) metodi koje se koriste u usluzi AZURE AD B2C i pomaže vam da odaberete NAJPRIKLADNIJI SSO metod prilikom konfigurisanja smernica.

**Koliko vremena traju? Koliko dugo traju?**

Token doћivotno je 1 sat i trajanje sesije je 24 časa. To znači da ako nije bilo zahteva za 24 časa, moraćete ponovo da se prijavite pre nego što zatražite novi simbol.

> [!NOTE]
> Posle 30 maja 2020, nijedan novi zakupac neće moći da koristi polisu životnog simbola za konfiguraciju za konfigurisanje sesije i osvežavanje simbola. Deprekacija će se desiti nekoliko meseci posle toga, što znači da ćemo prestati da poštićemo postojeće sesije i osvežavamo polise tikena. I dalje možete da konfigurišete oznaku za pristup ћivotna posle deprekacije.






