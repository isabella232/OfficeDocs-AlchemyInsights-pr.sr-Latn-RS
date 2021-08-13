---
title: Outlook Opoziv radne površine ili zamena e-poruke
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918409"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Opoziv ili zamena Outlook-poruke

- Kao korisnik možete da opozvane poruke u ime korisnika pomoću programa **PowerShell.** Poruke iz centra za adminise ne možete da opozvane.
- Možete **opozivati samo poruke koje su poslate osobama iz vaše organizacije.** Na primer, ako je poruka poslata na Gmail adresu, ne možete da je se setite.
- Možete da **opozvane samo poruke poslate sa računara Outlook 2016 sa računara.** Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na vebu, ne možete da je opozovete.

Da biste o opozovili ili zamenili e-poruku:

1. U oknu fascikle sa leve strane prozora Outlook izaberite fasciklu Poslate stavke.
1. Kliknite dvaput na poruku koju želite da opozozete da biste je otvorili.
1. Izaberite karticu **Poruka,** a zatim izaberite **stavku Radnje Opozovi** ovu  >  **poruku.**
1. Izaberite **Izbriši nepročitane kopije ove** poruke ili Izbriši nepročitane **kopije** i zameni ih novom porukom, a zatim kliknite na dugme **U redu.**
1. Ako šaljete zamennu poruku, sastavite poruku i izaberite stavku **Pošalji**.
1. Uspeh ili neuspeh opozivanja poruke zavisi od postavki primaoca u programu Outlook. Korake za proveru opoziva potražite u [ovom članku.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Traženje i brisanje e-poruka u organizaciji

- Ako niste globalni admini svom nalogu, morate da dodate svoj nalog u ulogu menadžera e-discikle ili ulogu upravljanja pretragom usaglašenosti da biste pretražili poruke. Da biste izbrisali poruke, morate da se pridružite grupi uloga "Upravljanje organizacijom" ili ulozi upravljanja pretragom i brisanjem. Dozvole za ove uloge dodeljene su u centru za [bezbednost i usaglašenost.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Kreirajte pretragu sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku za brisanje.
- [Povezivanje u PowerShell centar za bezbednost i usaglašenost.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Ako koristite višestruku potvrdu identiteta, pogledajte Povezivanje potvrdu Microsoft 365 bezbednost i usaglašenost programa [PowerShell pomoću višestruke potvrde identiteta.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)