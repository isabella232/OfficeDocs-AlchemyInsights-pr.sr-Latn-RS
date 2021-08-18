---
title: Omogućavanje pisanja lozinke u Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 607e27c883f83b4b29347e764b8f2273cf0f117e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325401"
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

Na **primer:** Kada administrator poništi korisnikove lozinke na Azure portalu, ako je taj korisnik federan ili heš lozinke sinhronizovan, ona se upisuje i dalje. Ova funkcionalnost zahteva licencu za Azure Premium (P1 ili P2) i trenutno nije podržana u Office portalu za administraciju.
