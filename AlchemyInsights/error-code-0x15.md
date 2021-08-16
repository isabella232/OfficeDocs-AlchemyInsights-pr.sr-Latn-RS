---
title: Kôd greške 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ako dobijate grešku prilikom aktivacije sistema Kancelarija 2013 u primenama usluge udaljene radne površine (RDS), razmotrite omogućavanje usluge ADAL tako što ćete urediti registrator.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100776"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Greška prilikom aktivacije Kancelarija 2013 u uslugama udaljene radne površine

Ako dobijate grešku prilikom aktivacije sistema Kancelarija 2013 u primenama usluge udaljene radne površine (RDS), razmotrite omogućavanje usluge ADAL tako što ćete urediti registrator.
  
|**Ključ registratora**|**Tip**|**Vrednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Više informacija potražite u [temi Omogućavanje moderne potvrde identiteta za Kancelarija 2013 na Windows uređajima.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL je podrazumevano omogućen u programima Microsoft 365 Apps za preduzeće i Kancelarija 2016. Usluge udaljene radne površine (RDS) su se ranije zvane Usluge terminala.
  