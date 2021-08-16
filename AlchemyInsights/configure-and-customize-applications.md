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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54045002"
---
# <a name="configure-and-customize-applications"></a>Konfigurisanje i prilagođavanje aplikacija

**Konfigurisanje aplikacija**

1. Brzi start: Konfigurisanje svojstava za aplikaciju [u Azure Active Directory (Azure AD) zakupca](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vam pokazuje kako da konfigurišete neka svojstva za aplikaciju.
2. Da bismo integrisali aplikacije sa Azure Active Directory [](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) programom, razvili smo kolekciju podučava koja će vas proći kroz konfiguraciju.
3. Konfigurisanje [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) aplikacije aplikacije vam pomaže da razumete kako da konfigurišete aplikaciju proxy aplikacije u okviru usluge Azure AD da biste izložili svoje aplikacije u oblak.
4. [Preuzmite PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)i konfigurišite aplikaciju: Pratite uputstva u *PingAccess za Azure A Microsoft Azure AD D* da biste zaštitili aplikacije objavljene korišćenjem proxyja aplikacije na veb lokaciji Ping Identity i preuzmite najnoviju verziju alatke PingAccess.

**Greške pogrešno konfigurisane aplikacije (AADSTS650056)**

1. Proverite da li pristupate aplikaciji sa adrese za prijavljivanje koju ste pružili vlasnik aplikacije. U suprotnom, prijavite se u aplikaciju putem normalnog procesa. U većini slučajeva ovo će se automatski razrešiti prirodno. Ako se ne reši, ova objava vam može pomoći da rešite probleme i probleme.
2. **Ako je vaša organizacija vlasnik aplikacije (što** znači da je registracija aplikacije u vašoj organizaciji):
    - Preporučujemo da se doda ili `User.Read` delegira `openid` dozvola od **korporacije Microsoft Graph.**
    - Uverite se da su za aplikaciju i sve njene dozvole pristanake. To možete da proverite tako što ćete pogledati **kolonu Status** registracije aplikacije u **okviru API dozvola.**
    - U nekim slučajevima, aplikacija može biti nezavisna organizacija, međutim, može biti registrovana u vašoj organizaciji. Potvrdite da li je ova aplikacija navedena u vašim registracijama za aplikacije (ne za Enterprise aplikacije).
    - Ako i dalje vidite ovu poruku o grešci. Zatim ćete možda morati da napravite URL adresu pristanka opisanu u **4. koraku.**
3. **Ako vaša organizacija nije vlasnik aplikacije i ako je koristi kao aplikaciju nezavisnog vlasnika:**
    - Ako ste administrator globalnog/preduzeća, trebalo bi da vidite ekran sa pristankom. Uverite se da ste u polju za **potvrdu "Pristanak u ime svoje organizacije".**
    - Ako ne vidite ekran sa pristankom, izbrišite Enterprise aplikaciju, a zatim pokušajte ponovo.
    - Ako i dalje vidite ovu poruku o grešci. Zatim ćete možda morati da napravite URL adresu pristanka opisanu u **4. koraku.**
4. Ručno napravite **URL** adresu pristanka koja će se koristiti: Ako je aplikacija dizajnirana za pristup određenom resursu, možda nećete moći da koristite dugmad za pristank sa Azure portala, morate ručno da generišete sopstveni URL adresu pristanka i da koristite ovo.
    - Potrebno je da nabavite `{App-Id}` i `{App-Uri-Id}` vlasnika aplikacije. `{Tenant-Id}` će biti identifikator zakuca. Ovo će biti ili `yourdomain.onmicrosoft.com` ID direktorijuma.
    - Ako se aplikacija pristupa samo za resurs, onda će `{App-Id}` i `{App-Uri-Id}` biti isti.
5. Više informacija potražite u temi Problemi sa prijavljivanjem u aplikacije konfigurisane za jedinstveno prijavljivanje zasnovane [na SAML-u.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Prilagođavanje aplikacija**

- Dodavanje [brendinga](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) na stranicu za Azure Active Directory za prijavljivanje organizacije – Koristite logotip i prilagođene šeme boja organizacije da biste obezbedili dosledan izgled i dosledan izgled stranicama za prijavljivanje u Azure Active Directory (Azure AD).
- [Dodajte prilagođeno ime domena](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) pomoću Azure Active Directory portala – Svaki novi Azure AD zakupca dolazi sa početnim imenom domena. Početno ime domena ne možete da promenite ili izbrišete, ali možete da dodate imena organizacije. Dodavanje prilagođenih imena domena vam pomaže da kreirate korisnička imena koja su poznata korisnicima.
