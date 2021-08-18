---
title: Razmena e-pošte putem sistema Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 8f8b0780ebec2911b6698deee25e0fabe83bd9afef5fb3a6ef4c51cccd67fc7c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898562"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Kako da podesite višefunkcionalni uređaj ili aplikaciju za slanje e-pošte

Da biste saznali koje opcije imate i koje korake treba da izvršite, pogledajte članak [Kako da podesite višefunkcionalni uređaj ili aplikaciju za slanje e-pošte pomoću sistema Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Ako imate uređaj ili aplikaciju koji su nedavno prestali da rade, najčešći problemi su:

- **Greške u vezi sa potvrdom identiteta prilikom korišćenja prosleđivanja SMTP Auth klijenta** Nedavno smo napravili neke promene u vezi sa načinom na koji funkcioniše SMTP potvrda identiteta. Više informacija o rešavanju problema potražite u odeljku "Potvrda identiteta bezuspešno" u odeljku Rešavanje problema sa štampačima, skenerima i aplikacijama za LOB koji šalju e-poštu pomoću Microsoft 365 ili [Office 365.](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)
- **Prihvatamo samo TLS 1.2 verziju i obezbeđujemo bezbednu vezu sa Office 365** Ako koristite bezbednu vezu (TLS), uverite se da uređaj aplikacije podržava TLS 1.2. Više informacija potražite u [temi Priprema za TLS 1.2](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)u Office 365 i Office 365 GCC.
 
Druge probleme i rešenja možete da pronađete u temi Rešavanje problema sa štampačima, skenerima i aplikacijama za LOB koji šalju e-poštu pomoću [Microsoft 365 ili Office 365.](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)

Da biste videli pogođene uređaje, idite na [Izveštaj o klijentima SMTP potvrde identiteta](https://protection.office.com/mailflow/dashboard).

**Napomi:** Exchange Online ne prati scenarije masovnog slanja. Da biste slali masovnu komercijalnu e-poštu (na primer, bištani klijenata), trebalo bi da koristite nezavisne dobavljače koji su specijalizovani za ove usluge.
