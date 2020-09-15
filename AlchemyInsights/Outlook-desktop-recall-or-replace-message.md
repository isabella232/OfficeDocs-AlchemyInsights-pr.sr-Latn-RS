---
title: Opoziv Outlook radne površine ili zamena e-poruke
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664004"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Opoziv ili zamena Outlook e-poruke

- Kao administrator, možete da **opozovete poruke u ime korisnika pomoću programa PowerShell**. Ne možete da opozovete poruke iz centra administracije.
- Možete da **opozovete poruke koje se šalju osobama u vašoj organizaciji**. Ako je poruka poslata na gmail adresu, na primer, ne možete da je opozovete.
- Možete **samo da opozovete poruke poslate iz programa Outlook 2016 na računaru**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na vebu, ne možete da ga opozovete.

Da biste opozvali ili zamenili e-poruku:

1. U oknu sa fasciklama na levoj strani prozora programa Outlook izaberite fasciklu poslate stavke.
1. Kliknite dvaput na poruku koju želite da opozovete da biste je otvorili.
1. Izaberite karticu **poruka** , a zatim izaberite **stavke Radnje**  >  **Opozovi ovu poruku**.
1. Izaberite stavku **Izbriši nepročitane kopije ove poruke** ili **Izbriši nepročitane kopije i zameni je novom porukom**, a zatim kliknite na **dugme u redu**.
1. Ako šaljete poruku za zamenu, sastavite poruku, a zatim izaberite stavku **Pošalji**.
1. Uspeh ili otkazivanje opoziva poruke zavisi od postavki primaoca u programu Outlook. Da biste proverili opoziv, pogledajte [Ovaj članak](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Pretraga i brisanje e-poruka u organizaciji

- Ako niste globalni administrator, nalog mora da se doda ulozi upravljača e-otkrivanja ili usaglašenosti u upravljanju potraživanju za pretraživanje poruka. Da biste izbrisali poruke, moraćete da se pridružite grupi uloga za upravljanje organizacijom ili svojoj ulozi za pretraživanje i čišćenje. Dozvole za ove uloge se dodeljuju u [centru za bezbednost i usaglašenost](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Kreirajte pretragu sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku za brisanje.
- [Povezivanje sa PowerShell centra za bezbednost i usaglašenost](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Ako koristite višestruku potvrdu identiteta, pogledajte članak [Povezivanje sa sistemom Microsoft 365 Security i Center za usaglašenost pomoću multifaktor potvrde identiteta](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).