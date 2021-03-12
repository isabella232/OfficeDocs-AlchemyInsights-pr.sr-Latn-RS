---
title: Problemi sa Microsoft Graph API-om
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714158"
---
# <a name="microsoft-graph-api-issues"></a>Problemi sa Microsoft Graph API-om

Ova tema može da se primenjuje i na programere koji i dalje koriste Azure AD Graph Graf. Međutim **, preporučuje se** da koristite Microsoft Graph za sve kataloge, identitete i Access scenarije upravljanja pristupom.

**Problemi sa autentikacijom ili autorizacijom**

- Ako aplikacija **ne može da dobije simbole** da bi pozvala Microsoft Graph, odaberite **problem sa prilikom dobijanja simbola za pristup (potvrda identiteta)** Microsoft Graph da bi se pribavila preciznije pomoć i podrška na ovoj temi.
- Ako aplikacija **prima 401 ili 403 greške autorizacije** prilikom pozivanja Microsoft dijagrama, izaberite kategoriju " **Preuzimanje zabrane pristupa" (autorizacija)** Microsoft Graph API za dobijanje specifične pomoći i podrške u ovoj temi.

**Želim da koristim Microsoft Graph, ali ne znam gde da počnem**

- [Pregled programa Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled identiteta i upravljanja pristupom u programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Prvi koraci u pravljenju Microsoft Graph aplikacija](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testiranje Microsoft Graph API-ja u zakupcu ili na demo zakupcu

**Želim da koristim Microsoft Graph, ali da li podržava API-ju usluge v 1.0?**

Microsoft Graph je preporučeni API za upravljanje katalogom, identitetom i Access upravljanju. Međutim, postoji nekoliko razmaka između onoga što je moguće u usluzi Azure A.D. i Microsoft Graph. Pregledajte sledeće članke koji naglašavaju najnovije razlike koje će vam pomoći u izboru:

- [Razlike tipa resursa između Azure reklama i Microsoft dijagrama](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike u svojstvima između Azure A.D. Grafa i Microsoft dijagrama](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike metoda između Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API koji zovem ne radi-gde mogu da uradim više testiranja?**

**Microsoft Graph Explorer** – testiranje Microsoft Graph API-ja u zakupcu ili na demonstracijuzakupcu i pročitajte **probne upite** u programu Microsoft Graph Explorer.

**Moja aplikacija je prespora i takođe se koristi. Koja poboljšanja mogu da napravim?**

U zavisnosti od scenarija, postoji mnoštvo opcija koje vam pripadaju na raspolaganju da biste aplikaciju načinili pristupačnijim, a u nekoliko slučajeva, manje sklon odbacivanjem usluge (kada pravite previše poziva).

- [Najbolje prakse za Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Zahtevi za sastanak](https://docs.microsoft.com/graph/json-batching)
- [Praćenje promena kroz Delta Query](https://docs.microsoft.com/graph/delta-query-overview)
- [Obaveštenje o promenama pomoću Veb-udica](https://docs.microsoft.com/graph/webhooks)
- [Usmeravanje smernica](https://docs.microsoft.com/graph/throttling)

**Gde mogu da pronađem više informacija o greškama i poznatim problemima?**

- [Informacije o odgovoru na Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Poznati problemi sa programom Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Gde mogu da proverim status raspoloživost usluge i vezu?**

Raspoloživost usluge i veza osnovnih usluga kojima se može pristupiti pomoću programa Microsoft Graph može da utiče na ukupnu dostupnost i performanse programa Microsoft Graph.

- Za Azure Active Directory zdravstveni sistem, potvrdite status **bezbednosti + usluge identiteta** navedenih na [stranici Azure status](https://azure.microsoft.com/status/).
- Za Office usluge koje doprinose programu Microsoft Graph, potvrdite status usluga navedenim na [kontrolnoj tabli usluge Office usluga](https://portal.office.com/adminportal/home#/servicehealth).

Greške Microsoft Graph autorizacije mogu da budu rezultat nekoliko raznih problema, od kojih većina stvara 401 ili 403 grešku. Na primer, sledeće mogu sve da dovedu do grešaka autorizacije:

- Neispravno [tokovi prikupljanja tokena za pristup](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Loše konfigurisani[opsezi dozvola](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Kraj podrške za Azure Active Directory biblioteku potvrde identiteta (ADAL) i Azure AD Graph API (AAD Graph)_* _

# * Počevši od 30 juna, 2020 * *, više nećemo dodavati nove funkcije u ADALE i Azure AD Graph. Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.

**Počevši od 30 juna, 2022**, završićemo podršku za Adale i AZURE AD Graf i neće više pružiti tehničku podršku ili bezbednosne ispravke.

Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće *dobiti tehničku podršku ili bezbednosne ispravke*.

Aplikacije koje koriste Azure AD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke Azure oglasa Graph.

**ADALA migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)koja ima najnovije funkcije i bezbednosne ispravke.

Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranja svojih aplikacija u MSAL pomoću krajnjeg roka za podršku, kada se osigura da će imati koristi od msalove trenutne bezbednosti i poboljšanja funkcija.

1. [Pročitajte najčešća pitanja za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saznajte više o tome kako da migrirate aplikacije na osnovu platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste Azure AD Graph, potražite uputstvo za [migraciju AZURE AD Graph grafika u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Naša lista za migraciju pruža tačku za početak](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph. Preporučujemo vam da pregledate sav izvorni kod aplikacija i, ako je primenljivo, kontaktirate bilo koje ISV-ove ili dobavljače aplikacija. Microsoft podrška vam takođe može pružiti listu svih podrške za AAD Graph u zakupcu.
3. Da bi aplikacija pristupala podacima u programu Microsoft Graph, korisnik ili administrator mora da joj dodeli ispravne dozvole putem procesa pristanka. [Referenca sa Microsoft Graph dozvolama](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph API. On takođe pruža uputstva o tome kako da koristite dozvole.
