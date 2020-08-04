---
title: Intune Wi-Fi profili
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555812"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi profili

Uspešna implementacija Wi-Fi povezanosti za klijente MDM zavisi od ispravnog rasporednog profila koji odražava zahteve korporativne Wi-Fi infrastrukture. Da biste pregledali odgovarajuće postavke za klijentske platforme koje istražujete, pogledajte: 

[Dodavanje Wi-Fi postavki za uređaje sa operativnim sistemom Android u programu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Dodavanje Wi-Fi postavki za Android Enterprise namenske i potpuno upravljane uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Dodavanje Wi-Fi postavki za iOS i iPadOS uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Dodavanje Wi-Fi postavki za Windows 10 i novije uređaje u Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Uvezi Wi-Fi postavke za Windows uređaje u usluzi Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Uobičajenih pitanja**

**Raspoređujem Wi-Fi profil koji zavisi od rasporednog certifikata navedenog u Wi-Fi profilu. Međutim, profili konfiguracije pokazuju status greške.**

Proverite da li je uređaj primio certifikat.

1. U Intune, idite na **sve uređaje** i izaberite uređaj > **Konfiguracija uređaja**.

2. Proverite da li su svi očekivani profili navedeni i u uspešnom stanju.

3. Ako imate posredničke certifikate u lancu certifikata, proverite da li su oni raspoređeni na Android uređaje.

    Da biste proverili status certifikata, idite na **profil konfiguracije uređaja**  >  **Profiles**  >  **Android srednji ca**  >  **Svojstva**  >  **pouzdani certifikat**.

Ako i dalje budete videli greške, pregledajte procedure i odeljke za rešavanje problema. Više informacija potražite u članku [pregled za Rješavanje problema sa SCEP profilima certifikata pomoću usluge Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Na uređaj sam rasporedio Wi-Fi profil. Intune pokazuje da je bila uspešna, ali uređaj se ne povezuje sa Wi-Fi.**

Uspešan status znači da je Intune uspešno rasporedila profil kao konfigurisan. Međutim, ove konfiguracije se možda ne podudaraju sa vašim mrežnim i/ili zahtevima za potvrdu identiteta. Za više detalja o Pokušani vezi, pregledajte evidencije u okviru usluge infrastrukture i potvrde identiteta (na kontroleru Wi-Fi pristupnih tačaka i NPS/radijus server). Možda ćete morati da radite sa mrežnim infrastrukturnim timom ili sa Wi-Fi dobavljačem nezavisnog proizvođača da biste prikupili i redigovali evidencije.