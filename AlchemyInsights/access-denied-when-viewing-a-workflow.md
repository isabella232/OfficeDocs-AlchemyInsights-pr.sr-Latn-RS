---
title: Pristup je odbijen prilikom pregledanja toka posla
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688816"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Pristup je odbijen prilikom pregledanja toka posla

SharePoint 2013 tokovi posla koji pokušavaju da pošalju e-poruku u SharePoint grupu mogu da ne uspeju sa porukom o grešci "pristup nije dozvoljen" Ako članstvo SharePoint grupe nije podešeno na sve.
  
 **Da biste rešili ovaj problem, uradite sledeće:**
  
 1. Omogućite svima da vide članove SharePoint grupe.
  
 2. Uklonite SharePoint grupu iz reda "za" ili "CC" e-pošte.
  
 3. Eksplicitno dodajte korisnike u red "za" ili "CC" Ako se vidljivost članstva ne može promeniti za SharePoint grupu.
  
Da biste videli više detalja, pogledajte [http neovlašćeno na/_vti_bin/Client.svc/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  