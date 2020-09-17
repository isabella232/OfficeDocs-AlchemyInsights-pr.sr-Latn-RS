---
title: Uslovno pristup sa Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807673"
---
# <a name="conditional-access-with-intune"></a>Uslovno pristup sa Intune

Korišćenje  **uslovnog pristupa**  pomoću Intune zahteva 3 koraka:

- Kreirajte  **smernice za usaglašenost**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) da biste definisali postavke koje moraju da se ispune da bi se uređaj smatrao usaglašenim. Na primer, uređaj mora da ima PIN od najmanje 6 cifara pre nego što se smatra usaglašenim.
- Kreiranje **uslovne smernice za pristup**  koja definiše resurse koji se čuvaju i koje uslove treba ispuniti da bi se pristupili te resurse.  [Na primer,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  uređaj mora da se usklaji pre pristupanja e-pošti preduzeća.
- Uverite se da su **smernice za usaglašenost**  i  **uslovne smernice za pristup**  usmereni na željene grupe korisnika. To može zahtevati Kreiranje određenih grupa korisnika u usluzi Azure Active Directory.

**Korisne veze:**

[Pregled usaglašenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rešavanje problema sa kom](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Smernice za rešavanje problema](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

Da biste zaštitili e-poštu (Exchange online) iz programa Access uređajima koji nisu usaglašeni, oba dokumenta moraju da se slede:

1. [Zaštita pristupa e-poštom sa uređaja pomoću EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Zaštita pristupa e-poštom sa uređaja pomoću modernih klijenata za potvrdu identiteta kao što je Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)