---
title: Nije moguće prijaviti se u Teams zbog greške autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038414"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Nije moguće prijaviti se u Teams zbog greške autologon.microsoftazuread-sso dot com:443

Ako je omogućen automatski SSO kao potvrda identiteta za O365, možda ćete intranet sajtovima morati da dodate URL „autologon.microsoftazuread-sso.com“.  Ako je on već dodat na pouzdane sajtove i ako se automatski SSO koristi, treba ga ukloniti sa pouzdanih sajtova.

Pregledajte [Kontrolnu listu za rešavanje problema sa automatskim SSO prijavljivanjem](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Pratite ove korake da biste dodali URL na listu intranet sajtova:

1. Otvorite Internet Explorer klikom na dugme **Start**. U polje za pretragu unesite Internet Explorer, a zatim na listi rezultata kliknite na stavku **Internet Explorer**.
2. Kliknite na stavku **Alatke**, a zatim na stavku **Internet opcije**.
3. Izaberite karticu **Bezbednost**.
4. Sada kliknite na stavku **Lokalni intranet sajtovi**, zatim na dugme **Sajtovi**, pa na dugme **Napredno**.
5. Unesite URL veb sajta i kliknite na dugme **Dodaj**.
6. Kada završite, kliknite na dugme **Zatvori**.

Više informacija potražite u članku [Dokumentacija za primenu automatskog SSO prijavljivanja za O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (obuhvata proces zasnovan na smernicama za dodavanje URL adresa intranet sajtovima u 3. koraku).
