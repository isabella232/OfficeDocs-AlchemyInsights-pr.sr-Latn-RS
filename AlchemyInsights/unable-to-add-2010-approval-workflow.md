---
title: Nije moguće dodati 2010 tok posla za odobravanje
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582861"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Nije moguće dodati 2010 tok posla za odobravanje

U Microsoft SharePoint kolekciji lokacija ne možete dodati globalno tok posla koji je moguće ponovo koristiti (kao što je "odobrenje-SharePoint 2010") u listu ili biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite osnovnu Web lokaciju kolekcije lokacija u programu SharePoint Designer 2013.
  
2. U okviru **objekti lokacije**izaberite stavku **Tokovi posla**. 
  
3. U **novom** odeljku trake **tokova posla** izaberite opciju **tok posla**koji je moguće ponovo koristiti. 
  
4. U obrascu **Kreiranje toka posla** koji je moguće ponovo koristiti unesite ime * * *Repair2010* * *. Za **tip platforme**izaberite stavku **SharePoint 2010 tok posla**, a zatim kliknite na dugme **u redu**. 
  
1. U odeljku **Sačuvaj** na traci **toka posla** izaberite stavku **Objavi**. 
  
2. U odeljku " **Upravljanje** " na traci **toka posla** izaberite opciju " **Objavi globalno**". U dijalogu za potvrđivanje koji se pojavljuje izaberite **"u redu"**. 
  
3. U Web pregledaču pronađite osnovnu Veb lokaciju kolekcije lokacija, a zatim pristupite **postavkama** \> **kolekcije**lokacija. Uključi/isključi funkciju **tokova posla** : 
  
· Ako je funkcija *aktivirana* , kliknite na dugme **"Deaktiviraj",** a zatim kliknite na dugme " **Aktiviraj**". 
  
· Ako je funkcija *deaktivirana* , kliknite na dugme " **Aktiviraj**". 
  
Za više informacija pogledajte sledeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

