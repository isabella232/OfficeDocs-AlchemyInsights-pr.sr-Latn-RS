---
title: UPN sinhronizacija je onemogućena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038126"
---
# <a name="upn-sync-disabled"></a>UPN sinhronizacija je onemogućena

Ako ste počeli da sinhronizujete sa uslugom Azure AD pre 30. marta 2016. godine, pokrenite sledeću Azure AD PowerShell cmdlet da biste omogućili UPN uslovno podudaranje samo za organizaciju:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN meko podudaranje automatski je uključeno za organizacije koje su započele sinhronizaciju sa Azure AD uključene ili posle 30. marta 2016.
  
Da biste saznali više o omogućavanju mekih podudaranja u UPN-u i drugim funkcijama sinhronizacije, pogledajte [Azure AD Povezivanje](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)funkcija usluge sinhronizacije.
  

