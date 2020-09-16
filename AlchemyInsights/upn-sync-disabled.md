---
title: UPN sinhronizacija je omogućena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749528"
---
# <a name="upn-sync-disabled"></a>UPN sinhronizacija je omogućena

Ako ste započeli sinhronizaciju sa Azure AD pre 30.2016, uradite sledeće Azure AD PowerShell cmdlet usluge da biste omogućili UPN Meki podudaranje samo za vašu organizaciju:
  
 **Funkcija for-Msoldirsyncfunkcije-Enablesoftprovoonupn-omogućavanje $True**
  
UPN meka podudaranje automatski se uključuje za organizacije koje su počele da se sinhronizuju sa uslugom Azure AD ili posle 2016 30.
  
Da biste saznali više o omogućavanju mekog podudaranja na UPN i drugim funkcijama sinhronizacije, pogledajte članak [funkcije Azure AD Connect sinhronizacija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

