---
title: Popravljanje Microsoft 365 nije uspelo pronalaženje povezanih licenci za Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069618"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Popravljanje Microsoft 365 aplikacije "Nije uspelo pronalaženje office licenci povezanih"

Ako primite ovu poruku, pokušajte sledeće:

1. Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama. Pogledajte [Microsoft 365 ULS i IP adresa.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Uklonite [i ponovo Kancelarija licencu za korisnika](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) na koje ovo utiče. 
3. Otvorite nalog aplikacija Office [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) sa svih postojećih korisničkih naloga.
4. Idite na Windows Postavke > **Nalozi**  >  **e-pošte &** naloge i uklonite sve radne naloge osim naloga na koji to utiče.
5. Idite na Windows Postavke > **Pristup poslovnim** ili školskim nalozima i prekinite vezu sa svim poslovnim nalozima osim naloga na  >  koji to utiče.
6. Uspostavite početnu Kancelarija aktivacije. [Saznajte kako.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Prijavite se](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomoću korisničkog naloga na koji ovo utiče.

Dodatna rešenja za rešavanje problema možete da pronađete u odeljku Greške sa nelicenciranim proizvodom i [aktivaciju u Kancelarija.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)