---
title: Podrška za Microsoft Defender za čuvara aplikacije Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584012"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Podrška za Microsoft Defender za čuvara aplikacije Microsoft Defender

Dizajnirano za Windows 10 i Microsoft Edge, Gardiska aplikacija koristi hardver-izolacioni pristup koji korisniku omogućava da se kreće na nepouzdani sajt iz izolovanog, hiper-V-omogućenog kontejnera, odvojen od sistema domaćina.

Administrativni administrator definiše listu pouzdanih Veb lokacija, resursa oblaka i unutrašnjih mreža. Kada korisnik poseti lokaciju koja nije na listi, Microsoft Edge će otvoriti lokaciju u kontejneru. To znači da ako se ispostavi da je lokacija zlonamerna, računar host će ostati zaštićen i da napadač neće doći do Enterprise podataka.

Instalacija proširenja u kontejneru je podržana kao Microsoft Edge verzija 81 i može se kontrolisati pomoću smernica. Adresa Updateula koja se koristi u smernicama za proširive smernice treba da se doda kao neutralan resurs u smernicama za izolaciju mreže koju koristi čuvar aplikacije.

Više informacija potražite u članku [Podrška za Microsoft Edge za gardu aplikacije Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).
