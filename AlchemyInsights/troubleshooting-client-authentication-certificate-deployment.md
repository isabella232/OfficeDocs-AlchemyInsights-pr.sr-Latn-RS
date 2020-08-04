---
title: Rešavanje problema sa primenom certifikata za potvrdu verodostojnosti klijenta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555811"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Rešavanje problema sa primenom certifikata za potvrdu verodostojnosti klijenta

Intune NDES/SCEP i PKCS/PFX profili certifikata se obično koriste zajedno sa drugim tipovima profila kao što su WiFi, VPN i e-pošta da bi korisnicima omogućio identitet korporacijskih resursa. Kada su ti tipovi profila povezani sa profilom certifikata klijenta, zavisi od uspešnog raspoređivanja tog profila.

Početno podešavanje infrastrukture i pridružena konfiguracija profila certifikata klijenta često zahtevaju rešavanje problema. Za Postepeni vodič za uspešno podešavanje NDES konektora i uputstva za rešavanje problema za izoliranje problema sa primenom certifikata, pogledajte: 

- [Konfigurišite infrastrukturu za podršku SCEP sa Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled za Rješavanje problema sa SCEP profilima certifikata pomoću usluge Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Koristite referentne skripte ljuske da biste proverili konfiguraciju. Više informacija potražite u članku [Intune skripte za verifikaciju konektora certifikata](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Drugih uobičajenih pitanja**

**Kada pokušam da instaliram priključak za Intune potvrde na server NDES Connector, dobijam poruku "nije moguće proveriti lozinku u zahtevu za certifikat. Možda je već korišćen. Pribavite novu lozinku za prosleđivanje sa ovim zahtevom. "**  

Ova poruka znači da je potrebno da pokrenete instalaciju sa konektorom za certifikat kao administrator.

U nekim okruženjima, serveri na kojima pokreće Intune certifikat moraju da koriste proxy server za povezivanje sa uslugom Intune, kao i da konektor certifikata mora da koristi proxy. U nekim okolnostima, NDES Connector zanemaruje konfigurisane proxy postavke i možda će biti neophodno da konfigurišete postavke proxy servera dok se radi u bezbednosnom kontekstu Localsistema. 
 
Rešenje je pokretanje programa Internet Explorer kao sistema i konfigurisanje proxy servera u programu IE. Nakon ponovnog pokretanja usluge Intune Connector, NDES konektor se povezuje sa Intune.

**Korisnički uređaji više ne primaju certifikate za SCEP iz NDES.**

Moguće je da je certifikat za potvrdu identiteta klijenta izdao na NDES server, a naveden za vreme instalacije NDES Connector je istekao ili je nestao. Da biste otklonili: 
 
1. Deinstalirajte NDES konektor.  
2. Koristite ove detalje da biste zahtevali novu potvrdu identiteta klijenta ili certifikat potvrde identiteta servera: 
 
    - Naziv subjekta: CN = spoljašnji FQDN  
    - Alternativno ime teme (potrebno je oboje): DNS = eksterni FQDN, DNS = interni FQDN 
 
3. Ponovo instalirajte NDES Connector sa novim certifikatom.