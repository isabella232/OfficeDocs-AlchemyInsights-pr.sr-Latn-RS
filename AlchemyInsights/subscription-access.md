---
title: Pristup pretplate
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
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807720"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Nije moguće prijaviti Azure za prijavljivanje zbog problema sa pregledom (pregledač se ne odaziva, nastavlja da se vrti, ne učita itd.)

Možda ćete imati problema sa nestankom. Proverite da li postoji trenutna nestanka: [Azure zdravstveni status](https://status.azure.com/status/history/).

Odjavite se sa svih aktivnih Azure sesija. Započnite privatno ili inkognito režim Veb pregledača.

Možete i da pokušate da osvežite pregledač, koristite drugi pregledač, izbrišete keš keširanja ako iznad ne funkcioniše.

Saznajte više: [Rešavanje problema sa prijavljivanjem](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Nije moguće pristupiti pretplatama**

Na sajtu [Azure](https://portal.azure.com/)uverite se da je u nalogu u gornjem desnom članku izabrana Azure direktorijum.

U [centru Azure naloga](https://account.windowsazure.com/Subscriptions)proverite da li je nalog koji se koristi administrator naloga.

Saznajte više: [Rešavanje problema sa pronađenih pretplata](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Nije moguće pristupiti istoriji naplata**

Administrator naloga mora da se uveri da se korisnik pristupa informacijama o naplati dodaje u Azure Active Directory kao korisnik gosta: [Dodavanje ili brisanje novog korisnika](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

Korisniku treba da se dodeli globalna uloga administratora: [Dodeli ulogu korisnicima](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Proknjižite ovo, korisniku može biti dat pristup naplate koristeći RBAC smernice: [Dodeli pristup naplata](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Preporučeni dokumenti**

-   [Ne mogu da se prijavim za upravljanje Azure pretplatom](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)