---
title: Rešavanje problema sa pristupom "zabranjen pristup"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704908"
---
# <a name="troubleshoot-access-denied-messages"></a>Rešavanje problema sa pristupom "zabranjen pristup"

Ako je neko dobio poruku "pristup je odbijen" u deljenoj fascikli u sistemu SharePoint, administrator kolekcije lokacija je možda omogućio "sistem zatvaranja korisnika lokacije sa ograničenom pristupom". Da biste isključili ovu opciju: 
  
1. Pronađite lokaciju, kliknite na ikonu postavke, a zatim izaberite stavku **Postavke sajta**.
    
2. U okviru **Administracija kolekcije lokacija** izaberite stavku **funkcije kolekcije lokacija**.
    
3. Pored **ograničenog režima zatvaranja dozvole za ograničenje korisnika**, kliknite na dugme **Deaktiviraj**.
    
Poruka "pristup odbijen" takođe može da se pojavi za deljene fascikle ako je lokacija lokacija za objavljivanje. Informacije potražite u članku [zabranjen pristup prilikom pristupanja deljenoj fascikli](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
Ako neko ima poruku "pristup nije dozvoljen" kada pokušate da prikažete zahteve za pristup, korisnik mora da se doda kao administrator kolekcije lokacija ili član grupe vlasnika za sajt. Više informacija potražite u članku [zabranjen pristup listi zahteva za pristup](https://go.microsoft.com/fwlink/?linkid=2004220).
  
Ako je korisnik dobio poruku "pristup je odbijen" nakon što su uklonjene iz aktivnog direktorijuma i ponovo dodata, pogledajte članak [zabranjen pristup kada se korisnički nalog sinhronizuje sa Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).
  

