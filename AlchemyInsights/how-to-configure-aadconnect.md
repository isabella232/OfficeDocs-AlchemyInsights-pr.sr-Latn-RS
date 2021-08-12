---
title: 646 Kako se konfiguriše AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963657"
---
# <a name="configure-sync-features"></a>Konfigurisanje funkcija sinhronizacije

Azure AD Povezivanje uključuje nekoliko funkcija koje su podrazumevano omogućene ili koje možete da omogućite kasnije. Neke funkcije zahtevaju dodatnu konfiguraciju u određenim okruženjima.

- [Ograničenja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) filtriranja, objekti se sinhronizuju sa Azure AD. Svi korisnici, kontakti, grupe i Windows 10 nalozi računara podrazumevano se sinhronizuju. Možete da uključite ili isključite objekte zasnovane na domenima, OU-ovima ili drugim atributima.

- [Sinhronizacija heša](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) lozinki sinhronizuje heš lozinke iz mera aktivnog direktorijuma sa aplikacijom Azure AD. To omogućava upravljanje lozinkom na jednoj lokaciji, ali korišćenje iste lozinke i u okruženjima u oblaku. Pošto je Active Directory ovlašćeni izvor, možete da koristite sopstvene smernice za lozinke.

- Samouslužno poništavanje lozinke [(SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogućava korisnicima da ponište sopstvene lozinke u oblaku, a da pri tom i dalje primenjuju lokalne smernice za lozinke.

- [Upisivanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) uređaja omogućava registrovanim uređajima u Azure AD da se upisuju u prenasedmu na sajtu Active Directory kako bi mogli da se koriste za uslovni pristup.

- Opcija Spreči slučajno brisanje podrazumevano je omogućena kao pomoć pri sprečavanju previše istovremenih [brisanja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) objekata (više od 500 objekata po sinhronizaciji). Ovu postavku možete da promenite kako biste ispunili potrebe svoje organizacije.

- [Automatska nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je podrazumevano omogućena za ekspresne instalacije i pomaže da se uverite da je vaša verzija usluge Azure AD Povezivanje uvek aktuelna.
