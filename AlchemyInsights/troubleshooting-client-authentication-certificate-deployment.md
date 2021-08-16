---
title: Rešavanje problema sa primenu certifikata za potvrdu identiteta klijenta
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
ms.openlocfilehash: 78520b416a72a3c93a3d2e7726948d59f83e681d4f09078c2a3cefac7bf1db3d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020818"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Rešavanje problema sa primenu certifikata za potvrdu identiteta klijenta

Profili certifikata Intune NDES/SCEP i PKCS/PFX klijenta često se koriste u isto vreme sa drugim tipovima profila kao što su Wifi, VPN i e-pošta kako bi se korisnicima omogućilo da potvrde identitet korporativnim resursima. Kada su ti tipovi profila povezani sa profilom certifikata klijenta zavise od uspešne primene tog profila.

Početno podešavanje infrastrukture i povezana konfiguracija profila certifikata klijenta često zahtevaju rešavanje problema. Za detalja vodič za uspešno podešavanje NDES konektora i uputstva za rešavanje problema u cilju izolacije problema sa primenom certifikata pogledajte: 

- [Konfigurisanje infrastrukture tako da podržava SCEP uz Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Pregled za rešavanje problema sa profilima SCEP certifikata sa Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Koristite referentne PowerShell skripte da biste verifikuli konfiguraciju. Više informacija potražite u članku [Skripte za intune certifikat za verifikaciju certifikata.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)

  
**Drugi uobičajeni problemi**

**Kada pokušam da instaliram konektor za Intune certifikat na NDES konektoru, dobijam poruku "Nije moguće verifikati lozinku u zahtevu za certifikat. Možda je već iskorišćena. Nabavite novu lozinku da biste je prosledili uz ovaj zahtev."**  

Ova poruka znači da kao administrator treba da pokrenete instalaciju konektora certifikata.

U nekim okruženjima, serveri u kojima je pokrenut Intune certifikat moraju da koriste proxy server za povezivanje sa uslugom Intune i zato konektor za certifikat mora da koristi proxy server. U nekim okolnostima, NDES Connector zanemaruje konfigurisane postavke proxy servera i možda je neophodno da se postavke proxy servera konfigurišu dok su pokrenuti u bezbednosnom kontekstu lokalnog sistema. 
 
Rešenje je da pokrenete Internet Explorer kao SISTEM i konfigurišete proxy server u programu IE. Nakon ponovnog pokretanja usluge Intune Connector, NDES Connector se povezuje sa uslugom Intune.

**Korisnički uređaji više ne primaju SCEP certifikate od korisnika NDES.**

Moguće je da je certifikat za potvrdu identiteta klijenta koji je izdao NDES server i naveden tokom instalacije NDES konektora istekao ili nedostaje. Da biste rešili: 
 
1. Deinstalujte NDES konektor.  
2. Koristite ove detalje da biste zatražili novu potvrdu identiteta klijenta ili certifikat za potvrdu identiteta servera: 
 
    - Ime teme: CN=spoljni fqdn  
    - Alternativno ime teme (oba su obavezna): DNS=spoljni fqdn, DNS=internal fqdn 
 
3. Ponovo instalirajte NDES konektor sa novim certifikatom.