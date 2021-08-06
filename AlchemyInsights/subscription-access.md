---
title: Pristup pretplatama
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999254"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nije moguće prijaviti Azure zbog problema sa pregledačem (pregledač se ne odaziva, ne učitava se itd.)

Možda će vas nešto uticati na preklonje. Proverite da li je došlo do trenutnog preklonjanja: [Azure status zdravstvenog stanja.](https://status.azure.com/status/history/)

Odjavite se iz svih aktivnih Azure sesija. Pokrenite režim privatnog ili incognito pregledača.

Možete da pokušate i da osvežite pregledač, koristite drugi pregledač, izbrišete kolačiće keša ako gorenavedeni ne funkcioniše.

Saznajte više: [Rešavanje problema sa prijavljivanjem](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nije moguće pristupiti pretplatama**

Na [portalu za Azure proverite](https://portal.azure.com/)da li je iz naloga u gornjem desnom vremenu izabran odgovarajući Azure direktorijum.

U [centru Azure naloga](https://account.windowsazure.com/Subscriptions)proverite da li je nalog koji se koristio administant naloga.

Saznajte više: [Rešavanje problema nije pronađeno nijedna pretplata](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nije moguće pristupiti istoriji naplate**

Korisnik naloga mora da proveri da li je korisnik koji pristupa informacijama o naplati dodat u Azure Active directory kao korisnik sa u goste: Dodajte ili izbrišite novog [korisnika.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

Korisniku zatim mora da bude dodeljena uloga globalnog adminisitera: [Dodeli ulogu korisnicima](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Ako objavite ovu objavu, korisniku može biti dodeljen pristup naplati pomoću RBAC smernica: [Odobrite pristup naplati](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Preporučeni dokumenti**

-   [Ne mogu da se prijavim za upravljanje Azure pretplatom](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)