---
title: Uslovni pristup sa intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069726"
---
# <a name="conditional-access-with-intune"></a>Uslovni pristup sa intune

Korišćenje  **uslovnog pristupa**  uz Intune zahteva 3 koraka:

- Kreirajte **smernice** za usaglašenost ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) da biste definisali postavke koje se moraju ispuniti da bi se uređaj smatrao usaglašenim. Na primer, uređaj mora da ima PIN kv od najmanje 6 cifara da bi se smatrao usaglašenim.
- Kreirajte **smernice za uslovni**  pristup koje definišu koji resursi se štite i koji uslovi treba da se zaduže da bi se pristupili tim resursima.  [Na primer, uređaj](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  mora da bude usavršan pre pristupa korporativnoj e-pošti.
- Uverite **se da su smernice**  za  **usaglašenost**  i smernice za uslovni pristup usmereni na željene grupe korisnika. Ovo može zahtevati kreiranje određenih grupa korisnika u programu Azure Active Directory.

**Korisne veze:**

[Pregled usaglašenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rešavanje problema sa ca](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Smernice za rešavanje problema](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Da biste zaštitili e-poštu (Exchange na mreži) od pristupa bez pristupa, oba dokumenta moraju biti praćena:

1. [Zaštita pristupa e-pošti sa uređaja pomoću EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Zaštita pristupa e-pošti sa uređaja pomoću modernih klijenata za potvrdu identiteta kao što Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)