---
title: Podešavanje DKIM-a sa prilagođenim domenima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332321"
---
# <a name="set-up-dkim-with-custom-domains"></a>Podešavanje DKIM-a sa prilagođenim domenima

Morate da objavite dva CNAME zapisa za svaki prilagođeni domen u DNS-u. Da biste to uradio, koristite sledeći format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
Na **primer:** **DomainGUID** je tekst sa leve strane **.mail.protection.outlook.com** u prilagođenom MX zapisu za prilagođeni domen (na primer, contoso-com za domen **contoso.com**). **InitialDomain je** domen koji ste koristili kada ste se upisali za Office 365 **(na primer, contoso.onmicrosoft.com**).

Više informacija o DNS zapisima potražite u temi [Pravljenje DNS zapisa kod bilo kog dobavljača usluga DNS hostinga za Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)