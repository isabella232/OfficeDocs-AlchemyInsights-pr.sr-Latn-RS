---
title: Brisanje sirotog korisnika sa servera na lokaciji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198589"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Brisanje sirotog korisnika sa servera na lokaciji

Da biste uklonili nesirotog korisnika, sledite ove korake:

1. Nametni sinhronizaciju direktorijuma prateći uputstva u [čemu je hibridni identitet sa Azure aktivnim direktorijumom?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Da biste proverili sinhronizaciju direktorijuma, pogledajte [Šta je hibridni identitet sa Azure aktivnim direktorijumom?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ako sinhronizacija ispravno funkcioniše, ali se Brisanje objekta aktivnog direktorijuma ne umnožava na Azure oglas, ručno uklonite nepovezani objekat koristeći jedan od sledećih Azure modula aktivnog direktorijuma za Windows PowerShell cmdlet:

    Ukloni-Msolkontakt  
    Ukloni-MsolGroup  
    Ukloni-MsolUser

    Na primer, da biste uklonili nedodeljena ID korisnika john.smith@contoso.com, originalno kreiran pomoću fascikle "sinhronizacija direktorijuma", pokrenite cmdpusti:

    Uklanjanje-MsolUser – korisnički Principalname John.Smith@Contoso.com