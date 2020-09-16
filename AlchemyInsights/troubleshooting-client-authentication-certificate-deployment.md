---
title: Rešavanje problema pri primeni certifikata identiteta klijenta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659000"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Rešavanje problema pri primeni certifikata identiteta klijenta

Intune/SCEPS i PKCS/PFX certifikati klijenata se najčešće koriste zajedno sa drugim tipovima profila kao što su WiFi, VPN i e-pošta da bi se korisnicima omogućio da potvrde potvrdu u korporacijske resurse. Kada su ovi tipovi profila povezani sa profilom certifikata klijenta zavise od uspešne primene tog profila.

Početna konfiguracija infrastrukture i povezana konfiguracija profila certifikata klijenta često zahtevaju rešavanje problema. Za vodič po koracima za uspešno podešavanje NDES konektora i uputstvo za rešavanje problema da bi se izoliram problemi sa primenom certifikata, pogledajte: 

- [Konfigurisanje infrastrukture za podršku pomoću Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled profila certifikata za rešavanje problema sa Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Koristite referentne scenarije da biste potvrdili konfiguraciju. Više informacija potražite u članku [skripte za verifikaciju konektora za verifikovanje certifikata](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Drugi uobičajeni problemi**

**Kada pokušam da instaliram konektor za potvrdu Intune na server NDES Connector, dobijam poruku "lozinka u zahtevu za certifikat ne može biti proverena. Možda je već korišćen. Nabavite novu lozinku za prosleđivanje sa ovim zahtevom. "**  

Ova poruka znači da treba da pokrećete instalaciju konektora za certifikat kao administrator.

U nekom okruženju, serveri na kojima je pokrenut certifikat Intune mora da koristi proxy server za povezivanje sa Intune tako da konektor za certifikat mora da koristi proxy. U odreрenim okolnostima, NDES konektor zanemaruje podešene proxy postavke i možda će biti potrebno da konfigurišu postavke proxy servera dok su u bezbednosnom kontekstu lokalnog sistema. 
 
Rešenje je da pokrećete Internet Explorer kao sistem i konfigurišete proxy u IE. Nakon ponovnog pokretanja usluge sistema Intune Connector, NDES konektor se povezuje sa Intune.

**Korisnički uređaji više ne primaju sertifikate iz funkcija NDES.**

Moguće je da je certifikat identiteta klijenta izdat NDES serveru i naveden tokom instalacije sistema NDES Connector, istekao ili da nedostaje. Da biste rešili: 
 
1. Deinstalirajte NDES Connector.  
2. Koristite ove detalje da biste zatražili novu potvrdu identiteta klijenta ili certifikat potvrde identiteta servera: 
 
    - Ime teme: CN = spoljni FQDN  
    - Alternativno ime subjekta (oba su potrebna): DNS = eksterni FQDN, DNS = interna FQDN 
 
3. Ponovno instaliranje NDES konektora pomoću novog certifikata.