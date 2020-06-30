---
title: Uslovni pristup sa Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931450"
---
# <a name="conditional-access-with-intune"></a>Uslovni pristup sa Intune

Korišćenje **uslovnog pristupa** sa Intune zahteva 3 koraka:

- Kreirajte **smernice usaglašenosti** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) da biste definisali postavke koje moraju da se ispune pre nego što se taj uređaj smatra usaglašen. Na primer, uređaj mora da ima PIN kôd od najmanje 6 cifara pre nego što se smatra usaglašen.
- Kreirajte **smernice za uslovno pristup** koje određuju koji resursi se štite i koji uslovi treba da budu ispunjeni da bi pristupili tim resursima.  [Na primer,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) uređaj mora biti usaglašen sa pristupom korporativnoj e-pošti.
- Uverite se da su **smernice za usaglašavanje** i **smernice uslovnog pristupa** usmerene na željene grupe korisnika. Ovo može zahtevati Kreiranje određenih grupa korisnika u Azure aktivnom direktorijumu.

**Korisni linkovi:**

[Pregled usaglašenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rešavanje problema CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Smernice za rešavanje problema](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Da biste zaštitili e-poštu (Exchange online) iz programa Access pomoću uređaja koji nisu usaglašeni, oba dokumenta moraju biti praćena:

1. [Zaštita pristupa e-pošti sa uređaja pomoću EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Zaštita pristupa e-pošti sa uređaja pomoću savremenih klijenata za potvrdu identiteta kao što je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)