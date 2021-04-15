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
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786863"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Predlozi za rešavanje grešaka "Nelicencivani proizvod"

Da biste rešili greške u vezi sa "Nelicencivan proizvod", pokušajte sledeće:

- Proverite da li je vaš status pretplate istekao.
- Proverite da li imate pretplatu koja omogućava licence klijenta, kao što su Microsoft 365 aplikacije za preduzeća ili Business Premium, i proverite da li je korisniku dodeljena [licenca](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Uverite se da se korisnik prijavava u Office sa istim nalogom koji ima dodeljenu licencu.
- Proverite [stranicu Zdravlje usluge](https://docs.microsoft.com/office365/enterprise/view-service-health) da biste videli da li postoje poznati problemi sa uslugom.
- Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne blokiraju pristup Microsoft 365 aplikacijama internetu. Pogledajte [UL adrese i opsege IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Možete da pokušate i sa sledećim radnjama za rešavanje problema: 

- Otvorite Office aplikaciju i [odjavite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) se sa postojećih korisničkih naloga. [Uklonite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [i ponovo dodelite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencu za Office, a zatim [se prijavite u Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomoću korisničkog naloga na koji ovo utiče.
- Pokrenite [alatku za rešavanje problema sa aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Uspostavite početne vrednosti stanja aktivacije sistema Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Obavite popravku na mreži sistema Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Dodatna rešenja za rešavanje problema potražite u članku: 

- [Greška „Nelicencirani proizvod“ i greška aktivacije u sistemu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [„Žao nam je, ne možemo da se povežemo sa nalogom. Pokušajte ponovo kasnije“ – greška prilikom aktiviranja sistema Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)