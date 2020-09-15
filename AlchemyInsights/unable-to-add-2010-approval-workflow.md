---
title: Nije moguće dodati 2010 tok posla za odobravanje
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699749"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Nije moguće dodati 2010 tok posla za odobravanje

U Microsoft SharePoint kolekciji lokacija ne možete da dodate globalni tok posla koji se može ponovo koristiti (kao što je "odobravanje-SharePoint 2010") na listu ili u biblioteku.
  
Da biste rešili ovaj problem, slijedite ove korake: 
  
1. Otvorite osnovnu Veb lokaciju kolekcije lokacija u sistemu SharePoint Designer 2013.
  
2. U okviru **objekti portala**izaberite stavku **Tokovi posla**. 
  
3. U **novom** odeljku trake **tokova posla** izaberite stavku **tok posla**koji je moguće ponovo koristiti. 
  
4. Na obrascu **toka posla** koji je moguće ponovo koristiti unesite ime * * *Repair2010* * *. Za **tip platforme**izaberite stavke **SharePoint 2010 tokovi posla**, a zatim kliknite na dugme **u redu**. 
  
1. U odeljku **Čuvanje** trake **toka posla** izaberite stavku **Objavi**. 
  
2. U odeljku **Upravljanje** traci **toka posla** izaberite stavku objavi na **globalnom nivou**. U dijalogu za potvrdu koji se pojavi izaberite stavku **u redu**. 
  
3. U Veb pregledaču pronađite osnovnu Veb lokaciju kolekcije lokacija, a zatim Access **Site Settings** \> **funkcije kolekcije lokacija**za postavke lokacije. Preklopnik funkcije **tokova posla** : 
  
· Ako je funkcija  *aktivirana*  , kliknite na dugme **Deaktiviraj,** a zatim kliknite na dugme **Aktiviraj**. 
  
· Ako je funkcija  *deaktivirana*  , kliknite na dugme **Aktiviraj**. 
  
Više informacija potražite u sledećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

