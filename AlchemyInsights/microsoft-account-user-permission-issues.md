---
title: Problem sa rešavanjem problema – Korisnik nije pronađen u direktorijumu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098184"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problem sa rešavanjem problema – Korisnik nije pronađen u direktorijumu

Ako korisnici dobijaju poruku o grešci "nije moguće pronaći korisnika" u direktorijumu, pokušajte ponovo tamo gde je Tip problema Korisnik nije u direktorijumu.

Sledeće korake možete dovršiti da biste rešili problem.

- Uverite se da je nalog koji je prihvatio poziv e-poštom isti nalog koji se koristi za kasnije prijavljivanje. Uverite se da korisnik koristi isti nalog da bi prihvatio pozivnicu i prijavio se na sajt. 

Više informacija potražite u članku Kako da upravljate pseudonimima za [Microsoft nalog da biste </a> upravljali Microsoft 365 za prijavljivanje.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Idite na svaku lokaciju na kojoj korisnik dobija grešku. 

Dodajte "/_layouts/15/people.aspx/membershipgroupid=0" (unutar dvostrukih navodnira) na kraj URL adrese sajta. 

Primer: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Izaberite korisnika sa liste.

- Izaberite **stavku Ukloni korisničke** dozvole sa trake. 
-  Ponovo dodajte korisnika i ponovo ga pošaite korisniku.

