---
title: Ažurirajte DNS zapise da biste zadržali Veb lokaciju sa trenutnim dobavljačem hostinga
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815799"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Ažurirajte DNS zapise da biste zadržali Veb lokaciju sa trenutnim dobavljačem hostinga

1. U Microsoft 365 centru administracije idite na stranicu **Podešavanje**  >  [domena](https://admin.microsoft.com/Adminportal#/Domains) i na listi domena izaberite domen koji koristite za Veb lokaciju.

2. Izaberite stavku **+ novi prilagođeni zapis** i unesite sledeće:

  - Za **tip DNS** unesite: **A (adresa)**

  - Za **ime hosta ili pseudonim**, otkucajte sledeće: **@**

  - Za **IP adresu**otkucajte STATIČNU IP adresu za Veb lokaciju na kojoj se trenutno nalazi (na primer,: 172.16.140.1).

    Ovo mora biti  *statična*  IP adresa za Veb lokaciju, a ne  *dinamična*  IP adresa. Proverite sa lokacijom na kojoj se vaša Veb lokacija nalazi kako biste se uverili da možete da dobijete statičnu IP adresu za javnu Veb lokaciju.

3. Izaberite stavku **Sačuvaj**.

Pored toga, možete da kreirate CNAME zapis da biste pomogli korisnicima da pronađu Veb lokaciju.
  
1. Izaberite stavku **+ novi prilagođeni zapis** i unesite sledeće:

  - Za **tip DNS** unesite: **CNAME (pseudonim)**

  - Za **ime hosta ili pseudonim**, otkucajte sledeće: **www**

  - Za **adresu na adresu**otkucajte potpuno određeno ime domena (FQDN) za Veb lokaciju (na primer, contoso.com).

2. Izaberite stavku **Sačuvaj**.
