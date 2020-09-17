---
title: Kako da omogućite besprekoran SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780541"
---
# <a name="how-to-enable-seamless-sso"></a>Kako da omogućite besprekoran SSO

Omogućite besprekoran SSO kroz [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Ako radite na novoj instalaciji usluge Azure AD Connect, odaberite stavku [Prilagođena instalacija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). Na stranici za **Prijavljivanje korisnika** odaberite opciju **Omogućavanje jedinstvenog prijavljivanja** .
  
Da biste potvrdili da ste ispravno omogućili besprekoran SSO:
  
1. Prijavite se u [administrativni centar Azure Active Directory](https://aad.portal.azure.com) kao globalni administrator.

2. U levom oknu izaberite stavku **Azure Active Directory** .

3. Potvrdite da je Nesmetna jedinstveno prijavljivanje **omogućena**.

Da biste saznali više, pogledajte [Azure Active Directory Nesmetna prijavljivanje: brzi početak](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  