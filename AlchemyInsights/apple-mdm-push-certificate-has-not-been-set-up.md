---
title: Nije podešen nijedan od jabuka MDM Push certifikata
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440012"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Nije podešen nijedan od jabuka MDM Push certifikata

Certifikat "Apple MDM" (poznat i kao Apple) nije konfigurisan za vašu pretplatu. Bez konfigurisanog, Apple MDM Push certifikata, ne možete da se prijavite i upravljate uređajima za iOS i Mac OS. Kada dodate certifikat u Intune, korisnici mogu da instaliraju aplikaciju "portal Company" kako bi ih upišu.

1. Izaberite **"slažem se".** da biste dali korporaciji Microsoft dozvolu da šalje podatke u Apple.

2. Izaberite **Preuzmi svoj CSR** zahtev za potpisivanje potvrda o potpisivanju zahteva za kreiranje certifikata "Apple MDM". Datoteka se koristi da bi se zahtijevale odnos poverenja sa portala za Push certifikata na Apple.

3. Izaberite opciju **Kreiraj vaš MDM Push certifikat** da biste otišli do portala "Push certifikata". Prijavite se koristeći ID jabuke kompanije, a zatim izaberite stavku **Kreiraj certifikat**. Izaberite **stavku Odaberi datoteku**, potražite datoteku zahteva za potpisivanje certifikata, a zatim odaberite stavku **Otpremi**. Na stranici za potvrdu izaberite stavku **Preuzmi** da biste preuzeli datoteku certifikata (. Pem) i sačuvajte datoteku lokalno.
 
**Napomena**: certifikat je pridružen ID-u jabuke koji je korišćen za njegovo kreiranje. Kao najbolja praksa, koristite ID kompanije jabuka za zadatke upravljanja i uverite se da poštansko sanduče nadgleda više od jedne osobe ili korišćenjem liste distribucije. Nikada nemojte koristiti lični ID jabuke. Koristite isti ID jabuke da biste obnovili Jabukovo uverenje na svakih 12 meseci.
 
4. Unesite ID jabuke koji se koristi za kreiranje vašeg Apple MDM Push certifikata. Zapišite ovaj ID kao podsetnik kada je potrebno da obnovite certifikat.

5. Idite na datoteku certifikata (. Pem), izaberite stavku **Otvori**, a zatim odaberite stavku " **Otpremi**". Pomoću Push certifikata Intune može da se prijavi i upravlja Apple uređajima.