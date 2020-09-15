---
title: Rad sa ličnim ID-ovi za iOS VIP aplikacije 1018
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
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688960"
---
# <a name="working-with-ios-vpp-applications"></a>Rad sa iOS VANP aplikacijama

Pročitajte [Kako da upravljate iOS aplikacijama kupljenim kroz program za disk jedinicu pomoću programa Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) da biste saznali više o funkcijama, ograničenjima i koracima za korišćenje Apple programa za kupovinu volumena i podrške za njega u Microsoft Intune.
  
 **Uobičajeni problemi:** "Za korisnike sam dodelila iOS VIPP aplikaciju, ali Instalacija nije uspela".
  
- To se može dogoditi ako se na jednom dobavljaču usluga upravljanja mobilnim uređajima koristi pojedinačni VIPP. VIP simboli iz Apple se mogu koristiti samo sa jednim dobavljačem. Ako ste koristili Office Token sa više dobavljača, morate ponovo da otpremate simbol za Intune.

- Instalacija takođe može da propadne ako ukupan broj instalacija premašuje broj licenci. Da biste prikazali izveštaj o korišćenju licenci, idite na stranicu **Intune licence za mobilne aplikacije** \> **App licenses** . Da biste saznali kako da povratite licence koristite, pogledajte [Ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
