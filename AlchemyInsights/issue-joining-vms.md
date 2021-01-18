---
title: Problem sa uključivanja funkcija Vims
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885663"
---
# <a name="issue-joining-vms"></a>Problem sa uključivanja funkcija Vims

Da biste rešili probleme koji se javljaju prilikom pokušaja pridruživanja funkcija Vims, obavite sledeće korake:

1. Pokušajte da se prijavite pomoću **UPN** formata (na primer "joeuser@contoso.com") umesto formata **Samaccountname** (' CONTOSO\joeuser ').
2. Uverite se da ste omogućili sinhronizaciju lozinki u skladu sa koracima *iznetim iz vodiča za* pokretanje.
3. Proverite da li korisnički nalog koji utiče na stavku nije spoljni nalog u Azure AD zakupcu. Spoljni korisnici ne mogu da se prijave u kontrolisani domen od kako Azure AD Domain Services Domain nije imala akreditive za takve korisničke naloge.
4. Ako je korisnički nalog koji utiče na utiču samo na korisnički nalog, uverite se da su korisnici promenili lozinku kada ste omogućili Azure AD Domain usluge domena. Ovaj niz prouzrokuje hašove akreditiva za generisane usluge Azure AD Domain.
5. Ako su korisnici koje utiču na korisnike sinhronizovane iz lokalnog direktorijuma, proverite da li je preporučeno izdanje Azure AD Connect konfigurisano da obavi kompletnu sinhronizaciju.
6. Ako problemi budu i dalje u okviru stavke 4. koraka, izvršite sledeće komande sa sinhronizovane mašine:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.