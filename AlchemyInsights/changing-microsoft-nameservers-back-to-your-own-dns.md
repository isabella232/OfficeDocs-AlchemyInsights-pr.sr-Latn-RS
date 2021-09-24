---
title: Povratak sa Microsoft servera imena na upravljanje sopstvenim DNS zapisima
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506971"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Povratak sa Microsoft servera imena na upravljanje sopstvenim DNS zapisima

Ranije ste promenili NS zapise tako da upućuju na Microsoft (ns1.bdm.microsoftonline.com), ali sada ste odlučili da sami upravljate DNS zapisima:

Na veb lokaciji registra domena vratite server imena na registar ili prethodnu postavku. Ako niste upoznati sa DNS-om, obratite se podršci u registru domena. Imajte na umu da prenošenje promenaservera imena može potrajati i do 48 sati. 

1. Na portalu Microsoft 365 za upravljanje idite na **Postavke** Domeni , potvrdite izbor u polju za potvrdu pored domena, a zatim izaberite stavku Upravljanje  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **DNS-om**. 

2. U čarobnjaku izaberite **stavku Dodajte svoje DNS zapise i** dovršite čarobnjak. Ovo menja način na koji se upravlja DNS-om, a zatim vam omogućava da dodate prilagođene DNS zapise potrebne da biste podržali izabrane usluge.

Umesto toga, ako ste promenili zapise servera imena u Microsoft i imate veb lokaciju, možete da dodate DNS zapise za veb lokaciju umesto da vratite servere imena. Više informacija potražite u temi [Ažuriranje DNS zapisa kako biste zadržli veb lokaciju sa trenutnim dobavljačem usluge hostinga.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


