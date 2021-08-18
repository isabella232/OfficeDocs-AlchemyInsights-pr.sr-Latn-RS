---
title: Automatsko šifrovanje e Office 365 poruka poslatih određenim domenima
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
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318862"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatsko šifrovanje e Office 365 poruka poslatih određenim domenima

1. U centru [Exchange za administaciju odaberite](https://outlook.office365.com/ecp/) **stavku pravila za protok pošte > .** 
2. Kliknite na **ikonu Novo (+),** a zatim izaberite stavku **Office 365 šifrovanje poruka i zaštitu prava na poruke.**
3. U **2010**, unesite ime pravila, na primer *Šifruj poruke poslate contoso.com.*
4. U **e-pošti Primenite ovo pravilo** ako je , **odaberite stavku > domen je**. 
5. Unesite ime domena, na **primer, contoso.com.**
6. Kliknite na **ikonu Dodaj (+),** a zatim kliknite na dugme **U redu.**
7. Pored polja **Uradite sledeće izaberite** stavku **Izaberi jedan.** 
8. U **padajunom meniju RMS predloška** izaberite stavku **Šifruj**, a zatim kliknite na dugme **U redu.** (Ako ne vidite ovu opciju, to znači da vaš plan ne uključuje automatsko šifrovanje. Ali možete da ga dodate!)
9. Odaberite bilo koji opcionalni izbor (odaberite bilo koji opcionalni izbor (od kojih mnoge možete da napravite u ovom trenutku, od kojih mnoge može da bude podrazumevana postavka radi pojednostavljivosti).
10. Kliknite na dugme **Sačuvaj**.

**Važno:** Uvek možete da se vratite i uredite ovo pravilo kasnije.

Dodatne informacije o kreiranju pravila za šifrovanje potražite u temi Definisanje pravila za protok pošte za šifrovanje [e-poruka u Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)