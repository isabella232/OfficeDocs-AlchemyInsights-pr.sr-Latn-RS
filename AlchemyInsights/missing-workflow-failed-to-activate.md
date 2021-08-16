---
title: Tok posla koji nedostaje nije uspeo da se aktivira
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065442"
---
# <a name="missing-workflow-failed-to-activate"></a>Tok posla koji nedostaje nije uspeo da se aktivira

U Microsoft SharePoint kolekciji lokacija ne možete dodati tok posla koji se može globalno ponovo koristiti (kao što je "Odobrenje – SharePoint 2010") na listu ili u biblioteku.
  
Da biste rešili ovaj problem, pratite ove korake: 
  
1. Otvorite osnovni veb sajt kolekcije lokacija u programu SharePoint Designer 2013.
  
2. U **okviru Objekti lokacije,** izaberite **Tokovi posla**. 
  
3. U **odeljku Novo** na traci **"Tokovi posla"** izaberite stavku Tok posla koji je **može ponovo da sekoni.** 
  
4. U **obrascu Kreiranje toka posla koji je moguće** ponovo uneti unesite ime ** *Popravka2010* **. Za **Tip platforme izaberite** stavku **SharePoint 2010** tok posla, a zatim kliknite na dugme **U redu.** 
  
1. U **odeljku Čuvanje** trake **toka posla** izaberite stavku **Objavi.** 
  
2. U **odeljku Upravljanje** na traci **toka posla** izaberite stavku **Objavi globalno.** U dijalogu za potvrdu koji se pojavi izaberite stavku U **redu.** 
  
3. U veb pregledaču pronađite osnovnu veb lokaciju kolekcije lokacija, a zatim pristupite lokaciji **Postavke** \> **funkcije kolekcije lokacija.** Zatim isključite funkciju **"Tokovi posla":** 
  
· Ako je funkcija *aktivirana, izaberite* **stavku Deaktivacija, a zatim** kliknite na dugme **Aktiviraj.** 
  
· Ako je funkcija *deaktivirana, kliknite* na dugme **Aktiviraj.** 
  
Dodatne informacije potražite u sledećem [članku.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

