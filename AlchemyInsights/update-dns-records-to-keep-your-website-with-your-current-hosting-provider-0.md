---
title: Ažuriranje DNS zapisa da bi se zadržao veb sajt sa trenutnim dobavljačem usluge hostinga
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007696"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Ažuriranje DNS zapisa da bi se zadržao veb sajt sa trenutnim dobavljačem usluge hostinga

1. Na Microsoft 365 centar administracije stranici Podešavanje domena i na listi domena izaberite domen koji koristite za   >  [](https://admin.microsoft.com/Adminportal#/Domains) veb lokaciju.

2. Izaberite **+ Novi prilagođeni** zapis i unesite sledeće:

  - Za **tip DNS unesite:** **A (Adresa)**

  - Za **polje Ime hosta ili pseudonim** otkucajte sledeće: **@**

  - Za **IP** adresu otkucajte statičnu IP adresu na kojoj se veb lokacija trenutno hostuje (na primer, 172.16.140.1).

    To mora biti  *statička*  IP adresa za veb lokaciju, a ne  *dinamička*  IP adresa. Proverite na lokaciji na kojoj se vaša veb lokacija hostuje da biste se uverili da možete da dobijete statičnu IP adresu za javnu veb lokaciju.

3. Izaberite **Sačuvaj**.

Pored toga, možete da kreirate CNAME zapis da biste pomogli klijentima da pronađu vašu veb lokaciju.
  
1. Izaberite **+ Novi prilagođeni** zapis i unesite sledeće:

  - Za **tip DNS unesite:** **CNAME (pseudonim)**

  - Za **polje Ime hosta ili pseudonim** otkucajte sledeće: **www**

  - Za **polje Upućuje** na adresu otkucajte potpuno kvalifikovano ime domena (FQDN) za veb lokaciju (na primer, contoso.com).

2. Izaberite **Sačuvaj**.
