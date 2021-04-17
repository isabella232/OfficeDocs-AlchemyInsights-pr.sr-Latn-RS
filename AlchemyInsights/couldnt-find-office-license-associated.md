---
title: Popravka Microsoft 365 aplikacija Nije moguće pronaći povezane licence za Office
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
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816502"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Popravljanje poruke "Nije moguće pronaći office licence povezane" za Microsoft 365 aplikacije

Ako primite ovu poruku, pokušajte sledeće:

1. Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama. Pogledajte [članak Microsoft 365 opsezi UL adresa i IP adresa.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
2. Uklonite [i ponovo dodignite Office licencu za korisnika](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) na koje ovo utiče. 
3. Otvorite Office aplikaciju i [odjavite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) se sa postojećih korisničkih naloga.
4. Idite na postavke operativnog > **Naloge** e-pošte & naloge i uklonite sve radne naloge osim naloga na koje  >  to utiče.
5. Idite na postavke operativnog sistema Windows > Pristup poslovnim ili školskim nalozima i prekinite vezu sa svim poslovnim nalozima osim naloga na  >  koji to utiče.
6. Uspostavite početne vrednosti stanja aktivacije sistema Office. [Saznajte kako.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)
7. [Prijavite se](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomoću korisničkog naloga na koji ovo utiče.

Dodatna rešenja za rešavanje problema možete da pronađete u odeljku Greške sa nelicenciranim proizvodom i [aktivaciju u programu Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)