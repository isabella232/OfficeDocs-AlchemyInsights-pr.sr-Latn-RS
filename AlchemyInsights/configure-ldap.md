---
title: Konfigurisanje LDAP
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
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885576"
---
# <a name="configure-ldap"></a>Konfigurisanje LDAP

Da biste konfigurisali LDAP, uradite sledeće:

1. Potvrdite zdravlje domena na lokaciji [Azure](https://aka.ms/aadds-health).
1. Uverite se da je dostupna važeća Azure reklama za pretplatu i da su omogućene usluge Azure AD Domain.
1. Certifikat potreban za omogućavanje sigurnog LDAP-a mora biti dobijen od pouzdanog autoriteta za izdavanje certifikata ili biti samostalni certifikat.
1. Uverite se da certifikat prati obavezna [uputstva](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Nevažeći certifikat**
1. Da biste obnovili certifikat, slijedite korake da biste kreirali novi certifikat i ponovo otpremili: [Konfiguriši LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Da biste rešili poznati problem sa sigurnim LDAP obaveštenjima u usluzi Azure Active Directory Services, pogledajte članak [rešavanje LDAP upozorenja](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
