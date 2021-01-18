---
title: Virtuelna konfiguracija sa uslugama AAD Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885648"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuelna konfiguracija sa uslugama AAD Domain

Virtuelna konfiguracija sa uslugama AAD Domain uključuje sledeće korake: 

1. Proveravanje zdravlja domena na Azure portalu https://aka.ms/aadds-health
2. Provera NSG za pravila koja blokiraju portove neophodne za sinhronizaciju u uslugama Azure AD Domain. https://aka.ms/aadds-networking
3. Uverite se da je virtualna mreža primenjena u istoj Azure oblasti kao i domen Azure AD Domain.
4. Obezbeđivanje postojećeg domena sa istim imenom domena dostupnom na virtualnoj mreži.

Više detalja o dizajnu potražite u članku razmatranje usluge Azure virtuelne mreže za podršku AAD uslugama domena, pogledajte članak [razmatranje virtuelne mreže](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

