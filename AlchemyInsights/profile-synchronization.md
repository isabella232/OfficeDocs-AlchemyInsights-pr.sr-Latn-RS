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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923658"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Kada se promene profila sinhronizuju sa SharePoint aplikacijom korisničkih profila?

SharePoint Online koristi zadatak Active Directory uvoza tajmera (AD uvoz) za uvoz korisnika i grupa u aplikaciju korisničkog profila. 
  
1. AD Uvoz sinhronizuje promene iz SharePoint online prodavnice direktorijuma sa aplikacijom korisničkih profila. Te promene se obrađuju u grupama.
    
2. Zadatak tajmera se pokreće dok se promene ne sinhronizuju.
    
> [!NOTE]
> Vreme koje treba da se pokrene tokom posla zavisi od broja promena koje treba obradite. Veliki broj promena traje duže. Ugovor o nivou usluga (SLA) navodi da će se promena za korisnika u SharePoint Online direktorijumu odražavati u aplikaciji za korisnički profil u 24 časa. 
  
[Više informacija o sinhronizaciji korisničkih profila u SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

