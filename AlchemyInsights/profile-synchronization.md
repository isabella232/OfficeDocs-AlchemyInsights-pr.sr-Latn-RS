---
title: Sinhronizacija profila
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320723"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kada se promene profila sinhronizuju sa SharePoint aplikacijom korisničkog profila?

SharePoint Online koristi zadatak Active Directory uvoza tajmera (AD uvoz) za uvoz korisnika i grupa u aplikaciju korisničkog profila. 
  
1. AD Uvoz sinhronizuje promene iz SharePoint Online directory prodavnice sa aplikacijom korisničkih profila. Te promene se obrađuju u grupama.
    
2. Zadatak tajmera se pokreće dok se promene ne sinhronizuju.
    
**Na umu:** Vreme potrebno za pokretanje zavisi od broja izmena koje treba da se obrade. Veliki broj promena traje duže. Ugovor o nivou usluga (SLA) navodi da će se promena za korisnika u SharePoint Online direktorijumu odraziti u aplikaciji za korisnički profil u 24 časa. 
  
[Više informacija o sinhronizaciji korisničkih profila u SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

