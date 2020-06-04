---
title: Ažurirajte DNS zapise da biste zadržali Web lokaciju sa trenutnim dobavljačem hostinga
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665774"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Ažurirajte DNS zapise da biste zadržali Web lokaciju sa trenutnim dobavljačem hostinga

1. U Microsoft 365 admin Center idite na stranicu " **Podešavanje**  >  [domena](https://portal.office.com/adminportal/home#/Domains) " i na listi domena izaberite domen koji koristite za svoju Web lokaciju.

2. Izaberite **+ novi prilagođeni zapis** i unesite sledeće:

  - Za **DNS tip** ENTER: **A (adresa)**

  - Za **ime domaćina ili pseudonim**upišite sledeće:**@**

  - Za **IP adresu**otkucajte STATIČNU IP adresu za svoju Web lokaciju na kojoj se trenutno hostuje (na primer, 172.16.140.1).

    Ovo mora da bude *statična* IP adresa za Web lokaciju, a ne *Dinamička* IP adresa. Proverite sa lokacijom na kojoj se nalazi vaša Web lokacija da biste se uverili da možete da dobijete statičnu IP adresu za svoju javnu Web lokaciju.

3. Kliknite na dugme **Sačuvaj**.

Pored toga, možete da kreirate zapis CNAME da biste pomogli klijentima da pronađu vašu Web lokaciju.
  
1. Izaberite **+ novi prilagođeni zapis** i unesite sledeće:

  - Za **DNS tip** unesite: **CNAME (pseudonim)**

  - Za **ime domaćina ili pseudonim**upišite sledeće: **www**

  - Da **biste dobili poene za adresu**, otkucajte potpuno kvalifikovano ime domena (FQDN) za vašu Web lokaciju (na primer, contoso.com).

2. Kliknite na dugme **Sačuvaj**.
