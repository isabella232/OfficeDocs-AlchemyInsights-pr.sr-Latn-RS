---
title: Microsoft Edge niska korisničkog agenta (radna površina)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: 9311f17298fff3fee3282fe05bd1ddcd02780a80097e86b29d56ffd575a9a571
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976015"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a>Microsoft Edge niska korisničkog agenta (radna površina)

Niske korisničkog agenta (UA) mogu se koristiti za otkrivanje verzije određenog pregledača koja se koristi u određenom operativnom sistemu. Kao i drugi pregledači, Microsoft Edge uključuje ove informacije u HTTP zaglavlje "Korisnički agent" svaki put kada zatraži zahtev za lokaciju. Informacijama o verziji pregledača možete da pristupite i putem programa JavaScript upitima za vrednost "navigator.userAgent".

Preporučujemo da veb projektanti koriste otkrivanje funkcija kad god je to moguće kako bi poboljšali održavanje koda, smanjili razlomak koda i eliminisali rizik od preloma koda u slučaju budućih ažuriranja niske UA.

Više informacija potražite u Microsoft Edge [Niska korisničkog agenta (radna površina).](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)