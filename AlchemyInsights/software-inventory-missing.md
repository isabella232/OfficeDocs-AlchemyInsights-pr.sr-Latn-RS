---
title: Zalihe softvera nedostaju ili su netačni
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676513"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Zalihe softvera nedostaju ili su netačni

Zalihe softvera u softveru Upravljanje pretnjama i ranjivim mestima (TVM) su lista poznatog softvera u organizaciji sa zvaničnim uobičajenim navodima platforme (CPE).

Softverski proizvodi bez zvaničnog CPE-a nisu objavili ranjivosti. Zalihe obuhvataju i detalje kao što su ime prodavca, broj slabosti, pretnje i broj izloženih uređaja.

Promene softvera na uređajima obično se odražavaju na bezbednosnim portalima u roku od dva sata. Međutim, ponekad može potrajati duže. Trenutno ne postoji način da se na silom sinhronizuje; ovo je tekuća neprekidna procena.

Ako ste napravili promenu softvera i promena se ne odražava ispravno na TVM nakon 5 časova, pratite ove korake:

1. Proverite odeljak sa dokazema softvera da biste razumeli kako je softver otkriven.
1. Uverite se da je softver podržan. Softver može biti vidljiv samo na nivou uređaja čak i ako ga Upravljanje pretnjama i ranjivim mestima. Međutim, dostupni su samo ograničeni podaci.
1. Korake za prijavu netačnosti sa portala možete da vidite u izveštaju ["Neprecizno"](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Na primer:** Izveštavanje o netačnosti sa MDE portala je jednostupni kanal za inženjering. Ako je problem hitan, otvorite tiket za podršku.

Više informacija potražite u temi [Softverski zalihe – Upravljanje pretnjama i ranjivim mestima.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)