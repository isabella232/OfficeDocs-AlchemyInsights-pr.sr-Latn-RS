---
title: Addressing Teams greška pri prijavljivanjem AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822001"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Addressing Teams greška pri prijavljivanjem AADSTS9000411

Prilikom prijave u Microsoft Teams, možda ćete dobiti grešku: Žao nam je, ali imamo problema sa prijavljivanjem u **AADSTS9000411: Zahtev nije ispravno oblikovan. Parametar "login_hint" se duplira.**

Da biste rešili ovaj problem, uverite se da su Microsoft Teams klijenti ažurirani. Dodatne informacije o ažuriranju klijenta potražite u članku [Ažuriranje usluge Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

Ako iz nekog razloga ne možete da ažurirate klijenta, odjavljanje klijenta će obrtati većinu kešnih podataka. Međutim, ako i dalje imate problema posle prijavljivanja/prijavljivanja, zatvorite Teams i obrišite keš klijenta tako što ćete uraditi sledeće:
1. Zatvorite Microsoft Teams.
2. Idite na: %appdata%\microsoft\teams i izbrišite sve datoteke.
3. Ponovo otvorite Microsoft Teams.
