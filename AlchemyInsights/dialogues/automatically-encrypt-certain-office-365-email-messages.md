---
title: Automatsko šifrovanje određenih Office 365 e-poruka
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526740"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Automatsko šifrovanje određenih Office 365 e-poruka

Možete automatski da šifrujete poruke koje korisnici šalju određenim spoljnim osobama ili organizacijama. Da biste to uradili, izvršite sledeće korake:

1. Iz [Exchange centra administracije](https://outlook.office365.com/ecp/)odaberite stavku **protok pošte > pravila**. 
2. Kliknite na **novu (+)** ikonu, a zatim izaberite stavku **primene Office 365 Message šifrovanje i zaštita prava na poruke**.
3. U **ime** unesite ime pravila, kao što je *šifrovanje poruka koje se šalju u DrToniRamos@gmail.com*.
4. U okviru **Primenjivanje ovog pravila ako**, odaberite **> primaoca ova osoba**. 
5. U prozoru **Izbor članova** izaberite ime osobe na koju želite da se prijavi šifrovanje, a zatim kliknite na dugme **Dodaj**. 
6. Kada završite sa dodavanjem korisnika, kliknite na dugme **u redu**.
7. Pored polja **uradi sledeće** , izaberite stavku **Izaberi jednu**. 
8. U padajućem meniju **RMS predloška** izaberite stavku **šifrovanje**, a zatim kliknite na dugme **u redu**. (Ako ne vidite ovu opciju, to znači da vaš plan ne podrazumeva automatsko šifrovanje. Ali možete da ga dodate!)
9. Odaberite opcionalnu selekciju (sa liste opcionalnih izbora koje možete da napravite u ovom momentu, od kojih se mnogi mogu ostaviti podrazumevanom postavkom za jednostavnost).
10. Kliknite na dugme **Sačuvaj**.

> [!IMPORTANT]
> Uvek možete da se vratite i uredite ovo pravilo kasnije.

Više informacija o kreiranju pravila za šifrovanje potražite u članku [Definisanje pravila toka pošte za šifrovanje e-poruka u sistemu Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

