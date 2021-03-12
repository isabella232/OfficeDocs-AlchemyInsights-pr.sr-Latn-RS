---
title: Korišćenje uslovnog pristupa sa Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749261"
---
# <a name="using-conditional-access-with-intune"></a>Korišćenje uslovnog pristupa sa Intune

Korišćenje uslovnog pristupa pomoću Intune zahteva 3 koraka:

- [Kreirajte smernice za usaglašenost da biste definisali postavke koje moraju da se ispune da bi se uređaj smatrao usaglašenim. Na primer, uređaj mora da ima PIN od najmanje 6 cifara pre nego što se smatra usaglašenim.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Kreiranje uslovne smernice za pristup koja definiše resurse koji se čuvaju i koje uslove treba ispuniti da bi se pristupili te resurse. Na primer, uređaj mora da se usklaji pre pristupanja e-pošti preduzeća.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Uverite se da su smernice za usaglašenost i uslovne smernice za pristup usmereni na željene grupe korisnika. To može zahtevati Kreiranje određenih grupa korisnika u usluzi Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Pročitajte više o...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
