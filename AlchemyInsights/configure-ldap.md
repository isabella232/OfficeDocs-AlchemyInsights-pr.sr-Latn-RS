---
title: Konfigurisanje LDAP-a
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090426"
---
# <a name="configure-ldap"></a>Konfigurisanje LDAP-a

Da biste konfigurisali LDAP, uradite sledeće:

1. Proverite dobro stanje domena na [Azure portalu.](https://aka.ms/aadds-health)
1. Proverite da li je dostupna važeća Azure AD pretplata i da je omogućena usluga Azure AD Usluge domena.
1. Certifikat potreban za omogućavanje bezbedne LDAP potvrde mora da se dobije od pouzdanog javnog autoriteta za certifikaciju ili da bude samo potpisani certifikat.
1. Uverite se da certifikat sledi [neophodna uputstva.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Nevažeći certifikat**
1. Da biste obnovili certifikat, pratite korake da biste kreirali novi certifikat i ponovo otpremite: [Konfigurišite LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Da biste rešili poznati problem sa Bezbednim LDAP upozorenjima u uslugama domena usluge Azure Active directory, pogledajte [otklanjanje LDAP upozorenja.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
