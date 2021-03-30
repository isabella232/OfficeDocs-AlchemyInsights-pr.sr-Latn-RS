---
title: Pomoć za podešavanje noćnog ekrana
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405179"
---
# <a name="help-with-the-night-light-display-setting"></a>Pomoć za podešavanje noćnog ekrana

Da biste saznali više o postavkama za noćni ekran, pogledajte [postavljanje ekrana za noćno vreme u operativnom sistemu Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Ako su opcije noćnog svetla zasivo u vašoj postavki, proverite upravljački program ekrana: 

1. Kliknite na polje za pretragu na traci zadataka i ukucajte **Upravljač uređajima**, a zatim u rezultatima **pretrage izaberite** stavku Upravljač uređajima.
1. Razvijte **video adaptere**. 

Nažalost, funkcija noćnog svetla nije dostupna ako uređaj koristi DisplayLink upravljački program ili upravljački program za osnovni prikaz.

Funkcija noćnog svetla koristi nedavne grafičke tehnologije, tako da ćete možda morati da ažurirate upravljački program ekrana:  

- Proverite da li postoje ispravke tako što ćete **ići na**  >  **početni ekran Postavke**  >  **ažuriranja &**  >  **Ispravke za Windows Update**  >  .  

ILI

- Posetite veb lokaciju podrške proizvođača hardvera da biste ručno preuzeli i instalirali najnovije upravljačke programe za prikaz.

## <a name="reset-night-light-in-the-registry"></a>Resetuj noćno svetlo u registratoru

Ako ažuriranje upravljačkog programa za ekran nije uspelo, možda ćete morati da uspostavite početne vrednosti noćnog svetla u registratoru.  

**Oprez:** Ovaj korak za rešavanje problema preporučuje se samo za napredne korisnike. Ako neispravno izmenite registrator, može doći do ozbiljnih problema. Radi dodatne zaštite, izađite iz rezervne kopije registratora pre nego što ga izmenite kako biste mogli da ga vratite ako dođe do problema.

1. U polju za pretragu otkucajte **regedit**, a zatim u rezultatima pretrage izaberite **stavku** Uređivač registratora.

1. Idite na sledeći ključ registratora: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Izvezite i izbrišite sledeći potključ:$$windows.data.bluelightreduction.bluelightreductionstate

1. Izvezite i izbrišite sledeći potključ:$$windows.data.bluelightreduction.settings

1. Ponovo pokrenite Windows i proverite da li su dostupne opcije noćnog svetla.


