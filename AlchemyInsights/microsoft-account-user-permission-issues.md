---
title: Rešavanje problema – korisnik nije pronađen u direktorijumu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725421"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Rešavanje problema – korisnik nije pronađen u direktorijumu

Ako korisnici primaju poruku o grešci "nije moguće pronaći korisnika" u direktorijumu, pokušajte ponovo da pokušate gde je tip problema korisnik.

Sledeći koraci mogu da se završe radi rešavanja problema.

- Uverite se da je nalog koji je prihvatio poziv e-pošte isti nalog koji se koristi za prijavljivanje kasnije. Uverite se da korisnik koristi isti nalog za prihvatanje pozivnice i prijavljivanje na sajt. 

Više informacija potražite u članku [Upravljanje pseudonimima za Microsoft nalog </a> radi upravljanja Microsoft 365 prijavljivanju](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Potražite sve stranice u kojima korisnik prima grešku. 

Dodavanje "/_layouts/15/osoba Le.aspx/membersigrupid = 0" (unutar dvostrukog navoda) do kraja URL adrese lokacije. 

Primer: https://< "stutoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Izaberite korisnika sa liste.

- Na traci izaberite stavku **Ukloni korisničke dozvole** . 
-  Dodajte korisnika i ponovo pošaljite poziv korisniku.

