---
title: 646 kako se konfiguriše AADConnect
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
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704503"
---
# <a name="configure-sync-features"></a>Konfigurisanje funkcija sinhronizacije

Azure AD Connect obuhvata nekoliko funkcija koje su podrazumevano omogućene ili koje možete da omogućite kasnije. Neke funkcije zahtevaju dodatnu konfiguraciju u određenim okruženjima.

- Ograničenja [filtriranja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) objekti se sinhronizuju sa uslugom AZURE AD. Svi korisnici, kontakti, grupe i Windows 10 nalozi su podrazumevano sinhronizovani. Objekte na osnovu domena, use ili drugih atributa možete da uključite ili isključite.

- [Sinhronizacija lozinki](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizuje hash lozinku iz lokalnog aktivnog direktorijuma u AZURE AD. To omogućava upravljanju lozinkama na jednoj lokaciji, ali korišćenje iste lozinke u lokalnim i Cloud okruženju. Budući da je Active Directory autoritativni izvor, možete da koristite sopstvene smernice za lozinku.

- [Samouslužno poništavanje lozinke (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) omogućava korisnicima da resetuju sopstvene lozinke u oblaku dok se primenjuju smernice za lokalne lozinke.

- [Ponovno upisivanje uređaja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) omogućava da se registrovani uređaji u usluzi AZURE AD vrati u lokalnu fasciklu Active Directory tako da mogu da se koriste za uslovno pristup.

- [Sprečavanje slučajno brišu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) se podrazumevano omogućava da se spreče previše istovremenih brisanja objekata (više od 500 objekata po sinhronizaciji). Ovu postavku možete da promenite da biste ispunili potrebe organizacije.

- [Automatsko nadogradnja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je podrazumevano omogućena za ekspresne instalacije i pomaže da se osigura da je vaša verzija usluge AZURE AD Connect uvek aktuelna.
