---
title: Rad sa iOS VPP Applications Rule Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083028"
---
# <a name="working-with-ios-vpp-applications"></a>Rad sa iOS VPP aplikacijama

Pročitajte Kako da upravljate [iOS](https://docs.microsoft.com/intune/vpp-apps-ios) aplikacijama kupljenim preko programa za količinsku kupovinu pomoću usluge Microsoft Intune da biste saznali više o funkcijama, ograničenjima i koracima za korišćenje Apple programa za količinsku kupovinu i podršci za njega u programu Microsoft Intune.
  
 **Uobičajeni problemi:** "Korisnicima sam dodelio iOS VPP aplikaciju, ali instaliranje nije uspelo."
  
- Do ovoga može doći ako se u više dobavljača upravljanja mobilnim uređajima koristi jedan VPP token. VPP tokeni iz usluge Apple mogu da se koriste samo sa jednim dobavljačem. Ako ste koristili VPP token sa više dobavljača, morate ponovo da otpremite token u Intune.

- Instalacija takođe može otkazati ako ukupan broj instalacija premašuje broj licenci. Da biste prikazali izveštaj o dozvoli za licence, idite na stranicu Licence za **Aplikacije za Intune** \>  Mobile. Da biste saznali kako da povratite licence koje se koriste, pogledajte [ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
