---
title: Automatsko šifrovanje određenih e-poruka iz sistema Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e050074f26025906561237c9ef487ed4743f93b1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322263"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatsko šifrovanje određenih e-poruka iz sistema Office 365

1. U centru [Exchange za administaciju odaberite](https://outlook.office365.com/ecp/) **stavku pravila za protok pošte > .** 
2. Kliknite na **ikonu Novo (+),** a zatim izaberite stavku Office 365 šifrovanje poruka zaštitu prava **na poruke.**
3. U **2010**, unesite ime pravila, na primer *Šifruj sve poruke.*
4. U **e-poruci Primeni ovo pravilo ako** odaberite stavku **[Primeni na sve poruke]**. 
5. Pored polja **Uradite sledeće izaberite** stavku **Izaberi jedan.** 
6. U **padajućem meniju RMS predloška** izaberite stavku **Šifruj**, a zatim kliknite na dugme **U redu.** (Ako ne vidite ovu opciju, to znači da vaš plan ne uključuje automatsko šifrovanje. Ali možete da ga dodate!)
7. Potvrdite izbor **u polju za potvrdu Nadgledaj ovo pravilo** nivoom ozbiljnosti, a zatim izaberite željeni nivo. Ako vaše preduzeće ima ugovorne obaveze da šalje šifrovane sve e-poruke, preporučujemo da zadate nivo **"Visoko".**
8. U **okviru Odaberite model za ovo pravilo** kliknite na dugme **Primeni.** 
9. Odaberite bilo koji opcionalni izbor (odaberite bilo koji opcionalni izbor (od kojih mnoge možete da napravite u ovom trenutku, od kojih mnoge može da bude podrazumevana postavka radi pojednostavljivosti).
10. Kliknite na dugme **Sačuvaj**.

**Važno:** Uvek možete da se vratite i uredite ovo pravilo kasnije.

Dodatne informacije o kreiranju pravila za šifrovanje potražite u temi Definisanje pravila za protok pošte za šifrovanje [e-poruka u Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

