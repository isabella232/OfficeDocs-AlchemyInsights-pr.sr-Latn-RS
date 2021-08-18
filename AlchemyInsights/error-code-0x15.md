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
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316700"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Greška prilikom aktivacije Kancelarija 2013 u uslugama udaljene radne površine

Ako dobijate grešku prilikom aktivacije sistema Kancelarija 2013 u primenama usluge udaljene radne površine (RDS), razmotrite omogućavanje usluge ADAL tako što ćete urediti registrator.
  
|**Ključ registratora**|**Tip**|**Vrednost**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Više informacija potražite u [temi Omogućavanje moderne potvrde identiteta za Kancelarija 2013 na Windows uređajima.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Napomi:** ADAL je podrazumevano omogućen u uslugama Microsoft 365 Apps za preduzeće i Kancelarija 2016. Usluge udaljene radne površine (RDS) su se ranije zvane Usluge terminala.
  