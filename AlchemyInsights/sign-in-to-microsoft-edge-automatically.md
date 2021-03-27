---
title: Automatsko prijavljivanje u Microsoft Edge
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
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398743"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatsko prijavljivanje u Microsoft Edge

Microsoft Edge koristi podrazumevani OS nalog za automatsko prijavljivanje korisnika u skladu sa načinom konfigurisanja uređaja korisnika. 

Scenariji svakog tipa konfiguracije uređaja i procesa zavisnog korisnika su opisani u nastavku:

- **Uređaj je hibridni/AAD-J:** Ova opcija je dostupna u operativnom sistemu Windows 10, operativnom sistemu Windows sa nižim nivoom i odgovarajućim verzijama servera. Korisnici se automatski prilaže svojim Azure Active Directory (AD)nalozima.
- **Uređaj je pridružen domenu:** Ova opcija je dostupna u operativnom sistemu Windows 10, operativnom sistemu Windows sa nižim nivoom i odgovarajućim verzijama servera. Prema podrazumevanim postavkama, korisnici sa nalozima domena nisu automatski prijavljeni; da biste omogućili automatsko prijavljivanje za njih, koristite **smernicu ConfigureOnPremisesAccountAutoSignIn.** Da biste omogućili automatsko prijavljivanje za korisnike koji imaju Azure AD naloge, razmotrite hibridno pridruživanje uređajima.
- Podrazumevani nalog operativnog sistema je **Microsoft** nalog: Ova opcija je dostupna u operativnom sistemu Windows 10 RS3 (verzija 1709, verzija 10.0.16299) i novijim verzijama. Malo je verovatno da će se scenario desiti na poslovnim uređajima. Međutim, ako je podrazumevani OS nalog Microsoft nalog, Microsoft Edge će se automatski prijaviti korisnika sa Microsoft nalogom.
 
 
