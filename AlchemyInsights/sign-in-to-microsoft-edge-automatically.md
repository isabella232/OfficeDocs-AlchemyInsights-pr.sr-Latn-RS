---
title: Automatsko prijavljivanje na Microsoft Edge
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678814"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatsko prijavljivanje na Microsoft Edge

Microsoft Edge koristi podrazumevani nalog OS za automatsko prijavljivanje korisnika u skladu sa načinom konfigurisanja uređaja. 

Scenariji svakog tipa konfiguracije uređaja i njegovog procesa prijavljivanja zavisnog korisnika opisani su u nastavku:

1. **Uređaj je hibrid/AAD-J**: Ova opcija je dostupna u operativnom sistemu Windows 10, sistemu sa više nivoa i odgovarajućim verzijama servera. Korisnici se automatski prijave pomoću Azure Active Directory (AD) naloga.
2. **Uređaj je pridružen domenu**: Ova opcija je dostupna u operativnom sistemu Windows 10, u operativnom sistemu Windows 10 i odgovarajućim verzijama servera. Korisnici sa nalozima domena se podrazumevano ne potpiše automatski; da biste omogućili automatsko prijavljivanje za njih, koristite smernice **konfiguracione** polise. Da biste omogućili automatsko prijavljivanje za korisnike sa Azure AD nalozima, razmotrite hibridno pridruživanje njihovim uređajima.
3. **Podrazumevani nalog OS je Microsoft nalog**: Ova opcija je dostupna u operativnom sistemu Windows 10 RS3 (verzija 1709, verzija 10.0.16299) i novije verzije. Nije moguće doći do scenarija na preduzećima uređajima. Međutim, ako je podrazumevani nalog OS Microsoft nalog, Microsoft Edge će automatski prijaviti korisnika pomoću Microsoft naloga.
 
 
