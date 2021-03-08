---
title: Automatsko šifrovanje usluge Office 365 e-pošte koje su poslate na određene domene
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526696"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Automatsko šifrovanje usluge Office 365 e-pošte koje su poslate na određene domene

1. Iz [Exchange centra administracije](https://outlook.office365.com/ecp/)odaberite stavku **protok pošte > pravila**. 
2. Kliknite na **novu (+)** ikonu, a zatim izaberite stavku **primene Office 365 Message šifrovanje i zaštita prava na poruke**.
3. U **ime** unesite ime pravila, kao što je *šifrovanje poruka koje se šalju u contoso.com*.
4. U okviru **Primenjivanje ovog pravila ako**, odaberite **primalac > Domain**. 
5. Unesite ime domena, kao što je **contoso.com**.
6. Kliknite na ikonu **Dodaj (+)** , a zatim kliknite na dugme **u redu**.
7. Pored polja **uradi sledeće** , izaberite stavku **Izaberi jednu**. 
8. U padajućem meniju **RMS predloška** izaberite stavku **šifrovanje**, a zatim kliknite na dugme **u redu**. (Ako ne vidite ovu opciju, to znači da vaš plan ne podrazumeva automatsko šifrovanje. Ali možete da ga dodate!)
9. Odaberite opcionalnu selekciju (sa liste opcionalnih izbora koje možete da napravite u ovom momentu, od kojih se mnogi mogu ostaviti podrazumevanom postavkom za jednostavnost).
10. Kliknite na dugme **Sačuvaj**.

> [!IMPORTANT]
> Uvek možete da se vratite i uredite ovo pravilo kasnije.

Više informacija o kreiranju pravila za šifrovanje potražite u članku [Definisanje pravila toka pošte za šifrovanje e-poruka u sistemu Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)