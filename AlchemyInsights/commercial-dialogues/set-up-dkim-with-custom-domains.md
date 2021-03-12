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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747638"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="b0ccc-102">Podešavanje DKIM sa prilagođenim domenima</span><span class="sxs-lookup"><span data-stu-id="b0ccc-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="b0ccc-103">Morate da objavite dva CNAME zapisa za svaki prilagođeni domen u sistemu DNS.</span><span class="sxs-lookup"><span data-stu-id="b0ccc-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="b0ccc-104">Da biste to uradili, koristite sledeći format:</span><span class="sxs-lookup"><span data-stu-id="b0ccc-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="b0ccc-105">**Domen** je tekst sa leve strane **. mail.Protection.Outlook.com** u prilagođenom MX zapisu za prilagođeni domen (na primer, comso-com za domen **contoso.com**).</span><span class="sxs-lookup"><span data-stu-id="b0ccc-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="b0ccc-106">**Inicialdomain** je domen koji ste koristili kada ste se prijavili za Office 365 (na primer, **contoso.onmicrosoft.com**).</span><span class="sxs-lookup"><span data-stu-id="b0ccc-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="b0ccc-107">Više informacija o DNS zapisima potražite u članku [Kreiranje DNS zapisa kod bilo kog dobavljača usluga DNS hostinga za Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="b0ccc-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>