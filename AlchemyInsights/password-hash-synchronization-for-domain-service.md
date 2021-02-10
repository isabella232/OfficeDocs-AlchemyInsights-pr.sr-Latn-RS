---
title: Sinhronizacija lozinki za uslugu Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177623"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Sinhronizacija lozinki za uslugu Domain

**Ako vam je instanca "Azure AD DS" upitna da omogućite sinhronizaciju hash sinhronizacije lozinki**

Nailazite na scenario u kojem koristite hibridno okruženje sa korisnicima sinhronizuju iz lokalnog Azure Active Directory Services domena (AD DS) okruženja. Ovaj scenario se susreće bez obzira na to da li ste sinhronizuju lozinke hash usluge u lokalnim OGLADIMA sa vašim Azure AD zakupcem.

**Uzrok**

To se dešava zato što Azure AD Connect po podrazumevanoj vrednosti ne sinhronizuje zastareli novi tehnološki LAN Manager (NTLM) i Kerberos hash lozinke koji su neophodni za Azure ADS.

**Privremeno rešenje** 

Trebalo bi da konfigurišete Azure AD Connect da biste sinhronizovali te lozinke koje su potrebne za NTLM i Kerberos potvrdu identiteta.

Kada se konfiguriše Azure AD Connect, pravljenje lokalnog naloga ili događaj promene lozinki takođe sinhronizuje hash nasleđene lozinke u Azure AD. Pogledajte [ovde](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) za više informacija o tome i za uputstva o tome kako se omogućava sinhronizacija lozinki u usluzi AZURE AD DS hibridna okruženja.