---
title: Problemi sa poljima
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917035"
---
# <a name="issues-with-tokens"></a>Problemi sa poljima

Da biste upravljali problemima koji se odnose na simbole, možete izvršiti sledeće korake:

1. Možete da navedete životni program za pristup, ID ili SEML Token koji izda Microsoft Platform identiteta. Možete da postavljate Token ћivotna za sve aplikacije u organizaciji, za aplikaciju za više stanara (multi-organizacija) ili za određenu uslugu usluge u organizaciji. Više informacija potražite u članku prikaz [simbola koji je moguće konfigurisati u Microsoft platformi identiteta (pregled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Access tokena omogućava klijentima da bezbedno pozivaju zaštićene Veb API, a Veb Apis ih koristi za obavljanje potvrde identiteta i autorizacije. Kao u OAuth specifikaciji, Access simboli su neprozirne niske bez skupa formata – neki dobavljači identiteta (IDPs) koriste GUID-ove, drugi koriste šifrovane blopove. Microsoft platforma za identitet koristi mnoštvo formata Token Access, u zavisnosti od konfiguracije API-ja koji prihvata Token. Da biste saznali kako vaš API može da proveri valjanost i koristi zahteve unutar simbola za pristup, pogledajte članak [Access simboli za pristup Microsoft platformoji](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Microsoft biblioteka autentifikacije (MSAL) podržava nekoliko tokova autentičnosti za korišćenje u razlicitim scenarijima aplikacije. Više informacija potražite u članku [protok identiteta](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. 2,0 kôd autorizacije Grant može da se koristi u aplikacijama koje su instalirane na uređaju da bi dobili pristup zaštićenim resursima, kao što je Veb APIs. Korišćenje aplikacije Microsoft Platform za identifikaciju u usluzi 2,0, možete da dodate pristup za prijavljivanje i API-ju mobilnim i aplikacijama za stone računare. Pogledajte [protok koda Microsoft identiteta i OAuth 2,0 autorske kodove](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) za kako da se direktno programiramo u odnosu na protokol u aplikaciji, pomoću bilo kog jezika.
5. OpenID Connect (OIDC) je protokol za potvrdu identiteta ugrađen na OAuth 2,0 koji možete da koristite da biste bezbedno prijavili korisnika u aplikaciju. Kada koristite funkciju OpenID povezivanja Microsoft identiteta, možete da dodate pristup aplikaciji prijavljivanje i API-ju u aplikacije. [Microsoft Microsoft Platform i OpenID protokol povezivanja](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) prikazuje kako se to radi nezavisno od jezika i opisuje kako se šalju i primaju HTTP poruke bez korišćenja Microsoft Open-Source biblioteka.
    - Krajnje tačka korisničkog informacija je deo OIDC standarda, dizajniranog da vrati tužbe o korisniku koji je potvrdio. Više informacija potražite u članku [krajnju tačku Microsoft identifikacione platforme korisničkog sadržaja](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Pozivanje Veb API-ja u Veb aplikaciju pomoću lokacije azuri AD i openid povezivanja](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) prikazuje kako da napravite MVC Veb aplikaciju koja koristi azuri AD za prijavljivanje pomoću programa openid Connect, a zatim pozovete Veb API u okviru identiteta potpisanog korisnika pomoću usluge tokena koji se dobija kroz OAuth 2,0. Ovaj uzorak koristi OpenID Connect ASP .net OWIN i ADVE .net.
6. [Konfigurišite aplikaciju da razotkrije Veb API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) – u ovom brzi početak, REGISTRUJETE Veb API pomoću Microsoft platforme identiteta i izložite ga klijentskim aplikacijama tako što ćete dodati primer. Registrovanjem Veb API i izlaženjem pomoću opsega, možete da pružite pristup na osnovu dozvoljenih dozvola njegovim resursima za ovlašćene korisnike i klijentske aplikacije koje pristupaju API-ju.
7. U usluzi Azure Active Directory B2C (Azure AD B2C), protok lozinki vlasnika resursa (ROPC) je OAuth standard potvrde identiteta. U ovom toku, aplikacija, poznata i kao stranka oslanjanja, razmena važećih akreditiva za simbole. Akreditivi imaju korisnički ID i lozinku. Vraćene ћetone su Token ID, Token pristupa i Token osvežavanja. Više informacija potražite u članku [Podešavanje davanja lozinki vlasnika resursa u usluzi Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

