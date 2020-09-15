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
description: Ako dobijate grešku prilikom aktiviranja sistema Office 2013 na udaljenom radnom računaru (RDS), razmotrite omogućavanje ADALA uređivanjem registratora.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709201"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Greška tokom aktivacije sistema Office 2013 za usluge udaljene radne površine

Ako dobijate grešku prilikom aktiviranja sistema Office 2013 na udaljenom radnom računaru (RDS), razmotrite omogućavanje ADALA uređivanjem registratora.
  
|**Ključ registratora**|**Zatim**|**Cenimo**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |120  <br/> |

Više informacija potražite u članku [Omogućavanje moderne potvrde identiteta za Office 2013 na Windows uređajima](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADALA je podrazumevano omogućena u Microsoft 365 aplikacijama za preduzeća i Office 2016. Usluge udaljene radne površine (RDS) prethodno su bile imenovane uslugama terminala.
  