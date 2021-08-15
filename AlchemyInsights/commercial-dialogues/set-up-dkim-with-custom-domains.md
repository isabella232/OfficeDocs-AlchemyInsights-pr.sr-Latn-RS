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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994837"
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
> [!NOTE]
> **DomainGUID** je tekst sa leve strane **.mail.protection.outlook.com** u prilagođenom MX zapisu za prilagođeni domen (na primer, contoso-com za domen **contoso.com**). **InitialDomain je** domen koji ste koristili kada ste se upisali za Office 365 (na **primer, contoso.onmicrosoft.com**).

Više informacija o DNS zapisima potražite u temi [Pravljenje DNS zapisa kod bilo kog dobavljača usluga DNS hostinga za Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)