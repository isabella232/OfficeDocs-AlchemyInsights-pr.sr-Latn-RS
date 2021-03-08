---
title: Podešavanje DKIM sa prilagođenim domenima
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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525418"
---
# <a name="set-up-dkim-with-custom-domains"></a>Podešavanje DKIM sa prilagođenim domenima

Morate da objavite dva CNAME zapisa za svaki prilagođeni domen u sistemu DNS. Da biste to uradili, koristite sledeći format:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **Domen** je tekst sa leve strane **. mail.Protection.Outlook.com** u prilagođenom MX zapisu za prilagođeni domen (na primer, comso-com za domen **contoso.com**). **Inicialdomain** je domen koji ste koristili kada ste se prijavili za Office 365 (na primer, **contoso.onmicrosoft.com**).

Više informacija o DNS zapisima potražite u članku [Kreiranje DNS zapisa kod bilo kog dobavljača usluga DNS hostinga za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).