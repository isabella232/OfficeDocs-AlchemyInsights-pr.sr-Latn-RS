---
title: Omogućavanje pisanja lozinke u Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093369"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Omogućavanje pisanja lozinke u Azure AD Connect

Da biste omogućili samouslužno poništavanje vraćanja, prvo omogućite opciju „vraćanje početnih usluga“ u usluzi Azure AD Connect. Na serveru Azure AD Connect, dovršite sledeće korake:

1. Prijavite se na Azure AD Connect server i pokrenite **Azure AD Connect** čarobnjaka za konfiguraciju.
2. Na stranici **dobrodošlice** kliknite na dugme **Konfiguriši**.
3. Na stranici **Dodatni zadaci** izaberite stavku **Prilagodi opcije sinhronizacije**, a zatim kliknite na dugme **Sledeće**.
4. Na stranici **Povežite se sa Azure AD** unesite akreditiv globalnog administratora za Azure zakupca, a zatim kliknite **Sledeće**.
5. Na stranicama za filtriranje **Povezivanje direktorijuma** i **Domen/OU**, kliknite na **Sledeće**.
6. Na stranici **Opcionalne funkcije** potvrdite izbor u polju pored stavke **Pisanje lozinke** i kliknite na dugme **Sledeće**.
7. Na stranici **Spremno za konfiguraciju**, kliknite na **Konfiguriši** i sačekajte da se proces završi.
8. Kada vidite da se konfiguracija završila, kliknite na **Izlaz**.

Uz omogućeno pisanje lozinke u Azure AD Connect, konfigurišite Azure AD SSPR za generisanje.  Da biste omogućili pisanje lozinke u usluzi SSPR, dovršite sledeće korake:

1. Prijavite se na Azure portal pomoću globalnog administratorskog naloga.
2. Potražite i izaberite stavku **Azure Active Directory**, kliknite na **Poništi lozinku**, a zatim kliknite na **Lokalna integracija**.
3. Postavite opciju za **Želite li da pišete lozinke na lokalnom direktorijumu?** na **„Da“**.
4. Postavite opciju za **Želite li da omogućite korisnicima da otključavaju naloge bez poništavanja lozinke?** na **„Da“**.
5. Kada budete spremni, kliknite na dugme **Sačuvaj**.

Više informacija potražite u članku [Omogući Azure Active Directory samouslužno poništavanje vraćanja u lokalno okruženje](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Kada administrator poništi korisničku lozinku na Azure portalu, ako je taj korisnik ujedinjen ili je sinhronizovan heš lozinke, lozinka se ponovo piše lokalno. Ova funkcionalnost zahteva licencu za Azure Premium (P1 ili P2) i trenutno nije podržana u Office portalu za administraciju.
