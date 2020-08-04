---
title: Problemi sa VPN vezom
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555747"
---
# <a name="vpn-related-issues"></a>Problemi sa VPN vezom

Uspešna implementacija VPN veze za klijente MDM zavisi od rasporednog profila koji tačno odražava zahteve VPN infrastrukture. Za odgovarajuće postavke za klijentske platforme koje istražujete, pogledajte: 

[Postavke Windows 10 i Windows holografskog uređaja za dodavanje VPN veza pomoću funkcije Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Dodavanje VPN postavki na iOS i iPadOS uređajima u usluzi Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Postavke za Android uređaje da biste konfigurisali VPN u Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Dodavanje VPN postavki na macOS uređajima u usluzi Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Ako vaš VPN profil koristi potvrdu identiteta zasnovanu na certifikatu, uverite se da su u uspešno raspoređene osnovne profile certifikata i potvrde identiteta klijenta povezani sa VPN profilom.

**Uobičajenih pitanja**

**Na uređaj sam rasporedio VPN profil. Intune pokazuje da je bila uspešna, ali uređaj se ne povezuje sa VPN mrežom.**

Uspešan status znači da je Intune uspešno rasporedila profil kao konfigurisan. Međutim, ove konfiguracije se možda ne podudaraju sa vašim mrežnim i/ili zahtevima za potvrdu identiteta. Pregledajte evidencije u usluzi "infrastruktura" i "usluga za potvrdu identiteta" (na VPN serveru i NPS/radijus server) za više detalja o pokušnoj vezi. Možda ćete morati da radite sa mrežnim infrastrukturnim timom ili VPN dobavljačem nezavisnog proizvođača da biste prikupili i redigovali evidencije.

**Kada podesim prilagođenu VPN za iOS, funkcija VPN aplikacije nije dostupna.**

VPN aplikacija za iOS uređaje u usluzi Intune je trenutno dostupna određenoj listi dobavljača i partnera, koji takođe moraju da ispunjavaju preduslove za certifikat pre konfigurisanja VPN aplikacije po aplikaciji. Više informacija potražite u članku [Podešavanje virtuelne privatne mreže (VPN) po aplikacijama za iOS/iPadOS uređaje u usluzi Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Za više informacija o svim tipovima VPN veza u usluzi Intune pogledajte odeljak [Kreiranje VPN profila za povezivanje sa VPN serverima u usluzi Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN na zahtev ne pokreće se kada se pristupi konfigurisanim domenom**

Da biste testirali automatsko VPN postavke, postavite sledeće vrednosti:

Želim da uradim sledeće: **procenite svaki pokušaj povezivanja** 

Odaberite da li želite da se povežete: **Poveži se ako je potrebno**

Kada korisnici pristupaju ovim domenima: ime **ciljnog** *domena*

Ako gorenavedena Konfiguracija nije uspešna, dodajte sledeći element:

Kada je ova URL adresa nedostupna, Nametni povezivanje VPN-a: **Badurl**