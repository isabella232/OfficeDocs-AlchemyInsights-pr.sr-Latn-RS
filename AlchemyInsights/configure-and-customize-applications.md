---
title: Konfigurisanje i prilagođavanje aplikacija
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063664"
---
# <a name="configure-and-customize-applications"></a>Konfigurisanje i prilagođavanje aplikacija

**Konfigurisanje aplikacija**

1. [Brzi Start: konfigurisanje svojstava za aplikaciju u usluzi Azure Active Directory (AZURE AD) stanar](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vam pokazuje kako da konfigurišete neka od svojstava za aplikaciju.
2. Da biste mogli da integrišete aplikacije sa uslugom Azure Active Directory, razvili smo [kolekciju obuka](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) koji će vas provesti kroz konfiguraciju.
3. [Konfigurisanje proxy servera aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) vam pomaže da razumete kako da konfigurišete aplikaciju proxy servera u okviru AZURE AD da biste izložili lokalne aplikacije oblaku.
4. [Preuzmite pingvin i konfigurišite aplikaciju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application): uradite uputstvo *da biste konfigurisali pingvin za for Azure AD da biste zaštitili aplikacije* objavljene pomoću Microsoft Azure AD aplikacije proxy servera na Veb lokaciji ping identitet i preuzimanje najnovije verzije pingaccess.

**Pogrešno konfigurisane greške aplikacije (AADSTS650056)**

1. Uverite se da pristupate aplikaciji sa adrese za prijavljivanje koju pruža vlasnik aplikacije. Drugačije značenje, prijavite se u aplikaciju kroz normalan proces. U većini slučajeva ovo će se normalno automatski rešiti. Ako ne radi, ova objava može da pomogne u rešavanju problema i njenom rešavanju.
2. **Ako je organizacija vlasnik aplikacije** (što znači da je registracija aplikacija u vašoj organizaciji):
    - Preporučujemo da `User.Read` `openid` dodate ili delegiranu dozvolu **Microsoft Grafa** .
    - Uverite se da je na aplikaciji i svim njenim dozvolama saglasnost. Ovo možete da potvrdite tako što ćete pogledati kolonu " **status** " u registraciji aplikacije u usluzi **API dozvolama**.
    - U nekoj od slučajeva, aplikacija može biti nezavisni, ali može biti registrovana u organizaciji. Potvrdite da li je ova aplikacija navedena u registraciji aplikacija (ne u preduzećima).
    - Ako i dalje vidite ovu poruku o grešci. Zatim ćete možda morati da napravite karticu pristanak opisan u **4**.
3. **Ako vaša organizacija nije vlasnik aplikacije i koristi je kao samostalnu aplikaciju**:
    - Ako ste administrator globalnog/preduzeća, trebalo bi da vidite ekran "pristanak". Uverite se da ste potvrdili izbor u polju za potvrdu **"pristanak u ime organizacije"**.
    - Ako ne vidite ekran za pristanak, izbrišite poslovnu aplikaciju i pokušajte ponovo.
    - Ako i dalje vidite ovu poruku o grešci. Zatim ćete možda morati da napravite karticu pristanak opisan u **4**.
4. **Ručno KREIRAJTE URL za pristanak koji će se koristiti**: ako je aplikacija dizajnirana za pristup određenom resursu, možda nećete moći da koristite dugmad pristanak sa Azure portala, moraćete ručno da generišete svoju URL adresu i koristite ovo.
    - Moraćete da nabavite `{App-Id}` i od `{App-Uri-Id}` vlasnika aplikacije. `{Tenant-Id}` će biti vaš identifikator zakupca. Ovo će biti `yourdomain.onmicrosoft.com` ili vaš ID direktorijuma.
    - Ako aplikacija pristupa sama sebi za resurs, onda `{App-Id}` `{App-Uri-Id}` će biti isti.
5. Više informacija potražite u članku [problemi sa prijavljivanjem na jednostrano podešene aplikacije zasnovane na Single prijavljivanju](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application).

**Prilagođavanje aplikacija**

- [Dodajte brendiranje u stranicu "Azure Active Directory Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) " – koristite logotip organizacije i prilagođene šeme boja da biste pružali prijavljivanje na stranice "Azure Active Directory" (AZURE AD).
- [Dodajte prilagođeno ime domena koristeći Azure Active Directory portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) – svaki novi AZURE AD stanar sa inicijalnim imenom domena. Ne možete da promenite ili izbrišete Početno ime domena, ali možete da dodate imena vaše organizacije. Dodavanje prilagođenih imena domena pomaže vam da kreirate korisnička imena koja su upoznata sa vašim korisnicima.
