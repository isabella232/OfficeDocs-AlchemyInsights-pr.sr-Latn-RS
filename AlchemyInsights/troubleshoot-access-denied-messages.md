---
title: Rešavanje problema sa porukama koje su odbijene za pristup
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939897"
---
# <a name="troubleshoot-access-denied-messages"></a>Rešavanje problema sa porukama koje su odbijene za pristup

Ako je neko dobio poruku "Pristup zabranjen" u deljenoj fascikli u SharePoint, administrator kolekcije lokacija je možda omogućio "Režim zaključavanja korisničke dozvole ograničenog pristupa". Da biste isključili ovo: 
  
1. Idite na sajt, kliknite na ikonu Postavke, a zatim izaberite stavku Lokacija **Postavke.**
    
2. U **okviru Administracija kolekcije** lokacija izaberite **stavku Funkcije kolekcije lokacija.**
    
3. Pored stavke **Režim zaključavanja korisničke dozvole ograničenog pristupa** izaberite **stavku Deaktivacija.**
    
Poruka o zabranjenom pristupu može da se pojavi i za deljene fascikle ako je lokacija lokacija lokacija za objavljivanje. Informacije potražite u [članku Pristup zabranjen prilikom pristupa deljenoj fascikli.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
Ako je neko dobio poruku "Pristup nije zabranjen" kada pokuša da prikaže zahteve za pristup, korisnik mora da se doda kao administrator kolekcije lokacija ili član grupe vlasnika lokacije. Više informacija potražite u članku [Lista zahteva za pristup zabranjen pristupu.](https://go.microsoft.com/fwlink/?linkid=2004220)
  
Ako je korisnik dobio poruku "Pristup nije zabranjen" pošto ga je uklonjen iz usluge Active Directory, a zatim ponovo dodao, pogledajte pristup odbijen kada se korisnički nalog sinhronizuje [sa uslugom Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)
  

