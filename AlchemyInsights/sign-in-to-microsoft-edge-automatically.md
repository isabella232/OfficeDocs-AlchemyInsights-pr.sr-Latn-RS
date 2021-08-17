---
title: Prijavljivanje u Microsoft Edge automatski
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
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050708"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Prijavljivanje u Microsoft Edge automatski

Microsoft Edge koristi podrazumevani OS nalog za automatsko prijavljivanje korisnika u skladu sa načinom na koji je konfigurisan uređaj korisnika. 

Scenariji svakog tipa konfiguracije uređaja i procesa zavisnog korisnika su opisani u nastavku:

- **Uređaj je hibridni/AAD-J:** Ova opcija je dostupna na Windows 10 nivoa Windows nivoa, kao i u odgovarajućim verzijama servera. Korisnici se automatski prijasnu sa svojim Azure Active Directory (AD)nalozima.
- **Uređaj je pridružen** domenu: Ova opcija je dostupna na Windows 10, nivoima Windows nivoa i odgovarajućim verzijama servera. Prema podrazumevanim postavkama, korisnici sa nalozima domena nisu automatski prijavljeni; da biste omogućili automatsko prijavljivanje za njih, koristite **smernicu ConfigureOnPremisesAccountAutoSignIn.** Da biste omogućili automatsko prijavljivanje za korisnike koji imaju Azure AD naloge, razmotrite hibridno pridruživanje uređajima.
- Podrazumevani nalog operativnog sistema je **Microsoft** nalog: Ova opcija je dostupna u verziji Windows 10 RS3 (verzija 1709, verzija 10.0.16299) i novijim verzijama. Malo je verovatno da će se scenario desiti na poslovnim uređajima. Međutim, ako je podrazumevani OS nalog Microsoft nalog, Microsoft Edge će se automatski prijaviti korisnika sa Microsoft nalogom.
 
 
