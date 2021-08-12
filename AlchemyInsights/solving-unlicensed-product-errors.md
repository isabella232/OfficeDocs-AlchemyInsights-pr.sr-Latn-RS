---
title: Rešavanje grešaka "Nelicencivani proizvod"
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
- "3412"
- "9001428"
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957114"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Predlozi za rešavanje grešaka "Nelicencivani proizvod"

Da biste rešili greške u vezi sa "Nelicencivan proizvod", pokušajte sledeće:

- Proverite da li je vaš status pretplate istekao.
- Proverite da li imate pretplatu koja omogućava licence klijenta, kao što su Microsoft 365 aplikacije za posao ili Business Premium, i uverite se da korisnik ima [dodeljenu licencu.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Uverite se da se korisnik prijavuje u Kancelarija istim nalogom koji ima dodeljenu licencu.
- Proverite [stranicu Zdravlje usluge](https://docs.microsoft.com/office365/enterprise/view-service-health) da biste videli da li postoje poznati problemi sa uslugom.
- Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne Microsoft 365 aplikacijama da pristupe internetu. Pogledajte [UL adrese i opsege IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Možete da pokušate i sa sledećim radnjama za rešavanje problema: 

- Otvorite nalog aplikacija Office [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) sa svih postojećih korisničkih naloga. [Uklonite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [i ponovo dodelite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencu Kancelarija, a zatim se [prijavite u Kancelarija](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) korisničkog naloga na koji to utiče.
- Pokrenite [alatku za rešavanje problema sa aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Uspostavite početnu Kancelarija aktivacije](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Popravka na mreži usluge Kancelarija](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Dodatna rešenja za rešavanje problema potražite u članku: 

- [Greška „Nelicencirani proizvod“ i greška aktivacije u sistemu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [„Žao nam je, ne možemo da se povežemo sa nalogom. Pokušajte ponovo kasnije“ – greška prilikom aktiviranja sistema Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)