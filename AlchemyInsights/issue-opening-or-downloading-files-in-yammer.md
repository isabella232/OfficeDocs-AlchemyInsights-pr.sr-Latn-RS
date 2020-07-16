---
title: Izdavanje ili preuzimanje datoteka na mreži Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148339"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Izdavanje ili preuzimanje datoteka na mreži Yammer

Classic Yammer podržava više opcija za otpremanje datoteka u poruke i grupe. U zavisnosti od mrežne konfiguracije, datoteke koje se podrazumevano skladište u sistemu SharePoint.

Birač datoteka na novoj mreži Yammer još uvek ne podržava sve opcije dostupne u klasičnom mreži Yammer. Buduća ispravka će dodati dodatne funkcije. Više informacija potražite u članku [Prilaganje datoteke ili slike na poruku razgovora o mreži Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Nije moguće otvoriti ili preuzeti datoteku**  

Datoteka može da se otpremi na Yammer, ali se takođe povezuje sa datotekom na SharePoint mreži. Prvo morate da utvrdite lokaciju datoteke da biste rešili problem. Ako je datoteka otpremljena na Yammer, ona će imati *. yammer.com URL. Uverite se da su zahtevane URL adrese i IP adrese deblokirale. Više informacija potražite u objavi bloga [koristeći čvrste šifrirane IP adrese za Yammer se ne preporučuje](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Proverite da li je korisnik koji ujedno i globalni administrator može da preuzme datoteku. Ako je datoteka privatna, možda ćete morati da koristite režim "privatan sadržaj". Više informacija potražite [u članku nadgledanje privatnog sadržaja na mreži Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Gosti i datoteke na nivou mreže na mreži Yammer na SharePoint mreži**  

[Gosti na mrežnom nivou na mreži Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) ne koriste "AZURE AD B2B" i interni su za uslugu Yammer, tako da ne mogu da pristupe datotekama Yammer uskladištenim u sistemu SharePoint. Kreirajte eksterni AAD B2B korisnik koji može da pristupi bibliotekama dokumenata na SharePoint mreži koristeći taj identitet. Za informacije o budućem Azure podršci za goste na mreži Yammer, podrška za goste na mreži za [poslovne korisnike (B2B) u usluzi Yammer Preview-uslovi i najčešća pitanja](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).