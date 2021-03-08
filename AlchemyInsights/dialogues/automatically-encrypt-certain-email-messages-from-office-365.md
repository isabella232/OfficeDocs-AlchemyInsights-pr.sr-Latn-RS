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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526762"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Automatsko šifrovanje određenih e-poruka iz sistema Office 365

1. Iz [Exchange centra administracije](https://outlook.office365.com/ecp/)odaberite stavku **protok pošte > pravila**. 
2. Kliknite na **novu (+)** ikonu, a zatim izaberite stavku **primene Office 365 Message šifrovanje i zaštita prava na poruke**.
3. U **ime**, unesite ime za pravilo, kao što je *šifrovanje svih poruka*.
4. U okviru **Primenjivanje ovog pravila ako**, odaberite **[primenjuje se na sve poruke]**. 
5. Pored polja **uradi sledeće** , izaberite stavku **Izaberi jednu**. 
6. U padajućem meniju **RMS predloška** izaberite stavku **šifrovanje**, a zatim kliknite na dugme **u redu**. (Ako ne vidite ovu opciju, to znači da vaš plan ne podrazumeva automatsko šifrovanje. Ali možete da ga dodate!)
7. Potvrdite izbor u polju za potvrdu **nadgledanje ovo pravilo pomoću nivoa ozbiljnosti** , a zatim izaberite željeni nivo. Ako vaše preduzeće ima ugovorne obaveze za slanje svih šifrovanih e-poruka, preporuиujem podešavanje nivoa na **najviša**.
8. U okviru **Odaberite model za ovo pravilo** kliknite na dugme **Primeni**. 
9. Odaberite opcionalnu selekciju (sa liste opcionalnih izbora koje možete da napravite u ovom momentu, od kojih se mnogi mogu ostaviti podrazumevanom postavkom za jednostavnost).
10. Kliknite na dugme **Sačuvaj**.

> [!IMPORTANT]
> Uvek možete da se vratite i uredite ovo pravilo kasnije.

Više informacija o kreiranju pravila za šifrovanje potražite u članku [Definisanje pravila toka pošte za šifrovanje e-poruka u sistemu Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

