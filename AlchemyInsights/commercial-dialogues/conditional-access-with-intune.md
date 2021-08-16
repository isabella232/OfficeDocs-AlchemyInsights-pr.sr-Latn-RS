---
title: Korišćenje uslovnog pristupa uz Intune
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
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005788"
---
# <a name="using-conditional-access-with-intune"></a>Korišćenje uslovnog pristupa uz Intune

Korišćenje uslovnog pristupa uz Intune zahteva 3 koraka:

- [Kreirajte smernice za usaglašenost da biste definisali postavke koje se moraju ispuniti da bi se uređaj smatrao usaglašenim. Na primer, uređaj mora da ima PIN kv od najmanje 6 cifara da bi se smatrao usaglašenim.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Kreirajte smernice za uslovni pristup koje definišu koji resursi se štite i koji uslovi treba da se zaduže da bi se pristupili tim resursima. Na primer, uređaj mora da bude usavršan pre pristupa korporativnoj e-pošti.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Uverite se da su smernice za usaglašenost i smernice za uslovni pristup usmereni na željene grupe korisnika. Ovo može zahtevati kreiranje određenih grupa korisnika u programu Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Pročitajte više o...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
